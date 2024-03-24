---
share: true
---

# TLDR
- Slightly undersize your boss based on the smallest O.D. of the insert
- When setting with a soldering iron, heat and depress only a millimeter or two and then release, let cool.
    - Found it was easier to get a consistent, controlled setting


# Designing for
- https://markforged.com/resources/blog/heat-set-inserts

Insertion guide
https://www.makerbot.com/professional/post-processing/inserts/
https://clevercreations.org/brass-threaded-inserts-plastic-3d-printing/

https://hackaday.com/2019/02/28/threading-3d-printed-parts-how-to-use-heat-set-inserts/

To accommodate displaced material, I suggest increasing the hole depth by about 50% of the insert length. This change ensures that the displaced plastic has somewhere to go and doesn’t fill up the cavity where the insert should be.

![Pasted image 20230213090630.png](./0%20-%20Attachments/Pasted%20image%2020230213090630.png)

#### 3D printing hole accuracy

Keep in mind that the holes you design in your CAD software always come out smaller when you 3D print them. This happens for various reasons. Most notably, after the plastic is laid down, it cools down and shrinks. But there are also other things that affect this, like [_faceting errors_ and _segment pausing_](https://hydraraptor.blogspot.com/2011/02/polyholes.html).

Long story short, if you want accurate holes when 3D printing, you need to size up the hole diameters a bit in CAD. I usually add **0.2mm extra**. This is a good place to start, but it can vary depending on the slicer that you use and how well your printer is dialed in.


### **What** length **of threaded inserts to use**

In general when working with brass threads, the recommendation is to use at least a thread length of 1.5x the diameter of the bolt. So if you are working with an M5 (5mm) bolt, you would use a section of thread of at least 7.5mm (5*1.5) or longer.


# Diameter
The holes need to be around the same diameter as the threaded insert, each about 0.1mm bigger or smaller than the next hole. 

So if the insert is about 4.0mm (excluding the knurling), you might end up with holes with diameters of 3.8mm, 3.9mm, 4.0mm, 4.1mm and 4.2mm.


m2x3x3.5 insert
- make hole diameter: 3mm
- make length 1.5x the length: (3 x 1.5)mm

M3x6x6 insert
- make hole diameter: 6mm
- make length: (6 * 1.5)