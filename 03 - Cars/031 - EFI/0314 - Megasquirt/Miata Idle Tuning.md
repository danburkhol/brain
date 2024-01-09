---
share: true
---

Good, long video on tuning MS3
https://youtu.be/-ln9-EyFwVY

Use Lambda? 1.0 = 14.7 afr

1. Using Idle VE, get fueling closer to target AFR

- You don't want a lot of timing to maintain idle, minimum timing as needed. 
    - Closer to 10deg

2. In `Idle Advance Settings`, set the idle timing advance table to 10deg across the board
    1. Turn off `Idle RPM Timing Correction`
        1. You'll notice idle timing stays static, find out why
            1. In his example, `Cold Advance` was taking out 5deg as shown in the datalog
            2. Set cold advance `at temp` to 0
    2. use "PID Idle Activation" 
3. Set the scales on `Closed-loop idle initial values` to be realistic along the desired idle speed. 
    1. These initial values are used to command the IACV in CL
    2. Set y axis max scale to 200 as it's CLT temp
    3. e.g. 750, 850, 900, 1000, 1400
4. `Idle Target Curve` set the max end to your target idle speed
5. `Idle RPM Timing Correction Curve` 
    1. Set timing delta to `-20` < 0 deg < `20`
    2. At 0 RPM difference from target, 0deg of timing added
    3. -100 RPM from target adds 20deg
    4. 100 RPM from target removes -20deg
6. Using the `Idle Target Curve` to raise your idle, adjust the `Close-loop idle initial values` to corresponding to an acceptable floating around 10deg idle 
7. Closed loop PID Gains = 1000
8. Dashpot adder adds in extra idle valve to prevent a hard idle drop
9. `1000 RPM` target while using A/C
    1. `700 min RPM` to allow A/C compressor to turn on for safety
    2. `Idle-up duty cycle` to increase idle valve opening to set rpm
    3. `Idle-up delay` delays the a/c compressor from turning on to give the idle valve system time to compensate smoothly

# Example timing
![CleanShot 2023-01-22 at 18.28.31.png](../../../0%20-%20Attachments/CleanShot%202023-01-22%20at%2018.28.31.png)


# Closed-Loop Idle Initial Values
Calibrating your idle initial values will improve your idle quality by setting the baseline duty cycle for a given target RPM. 
The objective is to set the initial values such that it's the minimum duty cycle required of the idle valve to reach your target RPM.

## Symptoms of uncalibrated initial idle values
- It takes too long (if ever) to reach target RPM. After lifting, the engine may idle high as it's initial value is such that it is letting too much air in. 
    - At runtime, the ECU will pull duty cycle to reach target RPM. But it is a slow process
- Stalling on lift
    - Not open enough in time to supply enough air to reach target rpm
- Inconsistent idle

## Finding your initial values
This is a technique I did. It's not the best but it gets you 90% there sitting in the driveway.

### Setup
1. Rescale your Closed-Loop Idle Initial Values table such that
    1. X-axis: 800rpm, 900rpm, 1000rpm, 1100rpm, 1200rpm
    2. Y-axis: 20degF, 50degF, 80degF, 110degF, 200degF
2. For each column, set a safe value for all rows to start.
    1. Look at your existing values and pick a reasonable value based off the existing table. 
    2. Skew your initial values higher, as it will be easier to tune a high idle and bring it down as opposed to a bogging, stalling engine.
    3. Your table will look something like this when you're done

![CleanShot 2023-01-22 at 18.13.10.png](../../../0%20-%20Attachments/CleanShot%202023-01-22%20at%2018.13.10.png)

4. Get the car warmed up and idiling. It will probably idle higher than usual for now.
5. Setup a graph view plotting the following
    1. RPM, Close Loop Idle Target RPM, Close Loop Idle RPM Error, and PWM Idle Duty

### Calibrating
>[!INFO] Be mindful of additional engine load from accessories when calibrating. If your cooling fans kick on, do not use any duty cycle values that occurred while the fan was ON. Remember, we are looking for the minimum duty cycle to operate the idle valve to allow enough air in the hit the target RPM.
- For this example, pretend we are targeting 800rpm.
- The procedure is the same for all target rpm ranges. 

1. Set your Closed-Loop Idle Target RPM, in this case, 800rpm
2. Open your graph view
3. Race the engine a bit and release the throttle
4. Monitor the PWM Idle Duty, we want to know the following:
    1. As the engine came to an initial idle, what was the duty cycle at this time?
    2. After the initial idle drop, the ECU should slowly reduce the duty cycle to reach the target RPM.
        1. Take note of the duty that the ECU landed on to reach target RPM
5. Take the difference of these two values and set your Initial Value to the result
    1. e.g. (Initial Duty - (Initial duty - actual duty to hit target)) = new initial
    2. Set the new value in the closed-loop-initial value for the appropriate column
6. Rinse and repeat until the engine consistently decelerates to your target RPM without overshooting or undershooting and fine-tune to preference

- Execute this procedure for the full range of initial idle values