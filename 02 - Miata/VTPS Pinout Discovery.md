---
title: Determine Vtps Pinout
date: 2021-11-07T11:20:29-05:00
slug: 2021-11-07-determine-vtps-pinout
type: posts
draft: true
categories:
  - default
tags:
  - default
github gist: https://gist.github.com/danburkhol/c66ccf0d0668ca531172932efa0264f5
share: true
---


**VTPS guide**

If you don’t want to just buy an adapter harness here is how you figure out what pin is what and re-pin your connector accordingly.

Label the pins 1,2,3 and take the resistance measurement between pins 1-2, 1-3, and 2-3 with the throttle fully closed and once fully open. Create a chart plotting this data.

There are three rules to follow to determine what pin is what.

1\. The resistance between 5V and GND will be constant with the throttle open and closed.

2\. The resistance between GND and SIGNAL will be low with the throttle closed and high with the throttle wide open

3\. The resistance between 5V and SIGNAL will be high with closed, low with the throttle wide open

Using these three rules you can determine which pin is which from your readings. Here’s an example when i had to figure out the pin out of my Kia vTPS.

- 1-3 Closed: 4.99, Open: 4.99
- 2-3 Closed: 1.204, Open: 4.36
- 1-2 Closed: 4.02, Open: 0.856

At this time we know each pin could be 5V, GND, or SIGNAL.

Possibilities: 

- Pin 1: 5V, GND, SIGNAL
- Pin 2: 5V, GND, SIGNAL
- Pin 3: 5V, GND, SIGNAL

We can see because of rule #1, Pin 1 and 3 are either 5V or GND so that means it’s impossible for Pin 2 to be 5V or GND. Thus we just found our SIGNAL pin.

Possibilities: 
- Pin 1: 5V, GND
- Pin 2: SIGNAL
- Pin 3: 5V, GND

Because of rule #2, resistance between GND and SIGNAL will be low with closed, high when open. The readings between pins 2 and 3 meet this criteria and since we know pin 2 is SIGNAL, that means pin 3 can only be the GND. Thus:

- Pin 1: 5V=
- Pin 2: SIGNAL
- Pin 3: GND

# References
- http://www.megasquirtpnp.com/docs/mspnp\_gP\_mm9093.php?isModel=1