---
share: true
---


# Parts
## Coil on plugs
Part Number: 90080-19015
OEM Ignition Coils (Set of 4) 2003 - 2008 Toyota Corolla Prizm | 90080-19015

https://www.amazon.com/Replacement-Chevrolet-9008019015-9008019019-9091902239/dp/B08KT3FRGD/ref=sr_1_6?dchild=1&keywords=90080-19015&qid=1625957765&refinements=p_85%3A2470955011%2Cp_72%3A1248861011&rnid=1248859011&rps=1&s=automotive&sr=1-6


[[https://www.amazon.com/gp/product/B07GVTB944/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1|No Splice COP connector]]

4 - Way Japanese coil on plug connector kit (Toyota # 90980-11885 , GM # 88974044 )
https://www.bmotorsports.com/shop/product_info.php/products_id/1667?osCsid=komo6eebfe2saeddofrlarlbq1

 **5 x Sumitomo HW / HX / DL / SL Sealed Series wire seal, green (20-16 AWG)**   
Part # CONN-00119

**5 x Sumitomo TS / SL Female Terminal 0.5 - 1.25 mm2 ( 20 - 16 AWG )**    
Part # CONN-11856

**1 x 4 - Way Japanese coil on plug connector housing (Toyota # 90980-11885 , GM # 88974044 )**     
Part # CONN-100307



https://www.miataturbo.net/useful-saved-posts-8/upgrading-coil-plugs-all-years-cop-writeup-12704/

More resources
http://miataturbo.wikidot.com/cop
https://omgpham.com/toyota-cops-coil-on-plugs

Pre-fabbed brackets
https://circuitdreamer.com/product/parts/engine/parts-engine-accessories-pulleys/rad-roadster-garage-star-toyota-coil-on-plug-mounting-plate/
http://trackspeedengineering.net/product_info.php/products_id/103


https://www.youtube.com/watch?v=xOc1NVG1N0o

If you have a 90-93 Miata, everything is similar but you'll need to connect to your igniter plug.

Shopping list:
Toyota Coil on Plugs 90080-19015, Qty 4 (made for many Toyota/Lexus cars from 2000 on, used is fine - $50)  If you buy new, get the real Denso (OEM) version not one of the many knockoffs: https://amzn.to/2YgLWoY

4 pin coil connector pigtails, Qty 4 - $10-12 from Amazon: https://amzn.to/2Ycg7xe
16 gauge AWG wire (assorted colors): https://amzn.to/2XtlSJN
For '94+ Miatas, PNP connector to car's harness - https://bit.ly/2DaD6C7


```
18-20 gauge

It is recommended to use an 18-20 **gauge wire** for each **coil**, and then tie them to a single 10-12 **gauge wire**. Pin D = Battery Ground. This high current ground should go to the battery or to a ground stud that is directly connected to the battery.
```

Bracket (Hardware store):
1.5 inch by 16 inches aluminum flat bar, 1/8 inch thick
M6-1.0 x 40mm flat head machine screw, Qty 4
M6-1.0 nylon lock nut, Qty 4
M6-1.0 cap nut, Qty 4

Tools used:
Drill
Countersink drill bit, 5mm or 3/8 inch 
1 inch bi-metal hole saw: https://amzn.to/2Yag5WX
1/4 inch drill bit
10mm socket
Phillips head screwdriver
ratchet
soldering iron: https://amzn.to/2YeasXM
60/40 rosin core solder: https://amzn.to/2Ft5BKU
heat shrink tubing: https://amzn.to/2X4lX7j
3M Super 88 electrical tape: https://amzn.to/2Xzlycs
Loom wrap, 1/4": https://amzn.to/2Xudc6c
Loom wrap, 3/8": https://amzn.to/2N85tGJ

OGPedxing is all about DIY, gadgets, and tools. #Miata #NAMiata

GarageStar mounting plate
https://fab9tuning.com/toyota-coil-on-plug-mounting-plate-90-2000/
- Designed for 90080-19015 and 90919-02239 coils

Another guide on COP install w/ pinouts
https://motorsport-electronics.co.uk/mazda-mx-5-cop-coil-on-plug-install/


1.6 to 1.8 Coil Swap
http://www.aus-cartalk.com/tech/1.6to1.8CoilSwap.htm

Purchasable products
http://trackspeedengineering.net/product_info.php/products_id/28

Another guide
https://roadsterzoku.wordpress.com/2015/08/25/toyota-cop-guide/

FlowForce - MIATA LS COIL WIRING HARNESS Guide
https://static1.squarespace.com/static/550d95d2e4b06c8c5d106915/t/5cda38f215fcc035b4e18ee4/1557805300693/FLOWFORCE-LS-COIL-HARNESS-GUIDE+5%3A2019.pdf


A Dummy's Guide to Miata ignition
http://www.rivercityroad.com/garage/ign_theory.html

#tachometer
Using TACHOUT from the ECU instead of being driven by the coils
https://www.miataturbo.net/mspnp-55/mspnp2-tach-malfunctioning-1-6-a-83339/
```
On a 1.6L, if youre using TACHOUT instead of the ignitor:

you can send it to the B/W wire on 2I. This brings the tach signal to the ignitor wiring.

There you must combine b/w and y/b as show above.

This brings the TACHOUT signal from the MS to the y/b wire. This is the wire that goes back to the dash tach.

There should be nothing else connected to the y/b wire--no coils, no 1K pullup in the diagnostics box.
```


[Megasquirt](Megasquirt.md) Install docs
http://www.megasquirtpnp.com/docs/mspnp_gP_mm9093.php?isModel=1

```
https://www.miataturbo.net/mspnp-55/ms2pnp-settings-sequential-spark-cops-85122/
You should have wired:

Cly 1 to Spark A - OEM (Brn/Yllw)
Cly 2 to Spark D - Pin 14
Cly 3 to Spark B - OEM (Brn)
Cly 4 to Spark C - Pin 15

Then you have to change the ignition settings from wasted spark to coil on plug of course.
```


Testing coils 

Spark A - Coil A - Cyl 3 
Spark B - Coil B - Cyl 1
Spark C - Coil C - Cyl 4
Spark D - Coil D - Cyl 2

Cyl 1 - Spark B - Wrong
Cyl 2 - Spark D - OK
Cyl 3 - Spark A - Wrong
Cyl 4- Spark C - OK

Should be
1,3,4,2
A,B,C,D

Cyl 1 - Spark A
Cyl 2 - Spark D
Cyl 3 - Spark B
Cyl 4 - Spark C

---
Swap pins 1 and 3 on the COP harness
???

Cyl 1 - Spark A
Cyl 2 - Spark D
Cyl 3 - Spark B
Cyl 4 - Spark C

# 04/18/2021
Coil A - Cyl 3
Coil B - Cyl 1
Coil C - Cyl 4
Coil D - Cyl 2

# Testing 2021-07-10
note: bad
Coil A | Cyl 3
Coil B | Cyl 1
Coil C | Cyl 4
Coil D | Cyl 2


