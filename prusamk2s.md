---
title: Prusa MK2S Kit Construction & Issues
description: Documenting assembly process and issues with the Prusa MK2S 3D-printer kit
display_gitinfo: false
header: /img/prusa/bedlevel-treefrog.jpg
permalink: prusamk2s
---

In November 2017 I decided to take the plunge into the world of 3D printing, and, after much online research decided to go with a Prusa. At the time Prusa had two main models on offer - the MK2S and the newly released MK3. Both printers are available as kits or pre-assembled. The price of the MK2S was around €150 lower than the MK3.

I decided to buy the MK2S because it seemed like a safer bet going with a printer design that had been around longer and whose issues were known. I also decided to purchase the kit rather than the pre-assembled printer, under the advice of my friend Jarno - who is a 3D printer fanatic (and a huge fan of Prusa Research). Jarno recommended getting a kit because the assembly process of the printer is and important way to 'know your machine', this DIY know-how would be especially important later for tweaking and calibrating the printer.

## Assembly Manual
My printer arrived promptly in the first week of November and I started the first weekend I could building it. The kit itself comes with a detailed assembly manual - I found Prusa's [online MK2S manual](http://manual.prusa3d.com/c/Original_Prusa_i3_MK2S_kit_assembly) to be an extremely valuable resource. Every step includes tips from the user community for how to improve the assembly experience - which saved me a few times from making mistakes.

## (Step 7) X-end Idler Assembly Troubles

At [step 7](http://manual.prusa3d.com/Guide/3.+X-axis+assembly/299#s5109) of the X-axis assembly I hit a problem. In this step you have to insert a hexagonal nylock nut into a hexagon-shaped groove on a 3D-printed part, however the nut would not fit into the groove at all. Some commenters on the assembly manual were also having issues with this step - apparently the tolerance on these 3D-printed parts isn't so good.

One comment advised trying to push in the nut with pliers while tightening the M3 hex bolt from the other side. So I gave this a try. However, this didn't get the nut into its groove - rather, I heard a pretty disheartening **crack** --- which was the sound of the bolt head breaking through the plastic of the part and trapping the bearing+pulley wheel inside!

#### Here's the bearing stuck after the hex screw did its damage...

<img src="img/prusa/broken-x-end-idler01.jpg" alt="X-end Idler" style="width: 300px;"/>

<img src="img/prusa/broken-x-end-idler02.jpg" alt="X-end Idler" style="width: 600px;"/>

### Solution to the broken x-end idler...

As a solution I tried filing away the broken plastic inside the part and using a countersunk M3 screw, plus a washer to keep the screw from falling into the hole.

At this point I haven't finished assembling the kit yet, so I'm not sure if this 'fix' will cause some issues later when I start printing and calibrating. But overall it seems to be quite sturdy and the screw is nearly flush with the part.

#### Here's the mess after removing the bearing:

<img src="img/prusa/broken-x-end-idler03.jpg" alt="X-end Idler" style="width: 600px; align: left;"/>

<img src="img/prusa/broken-x-end-idler04.jpg" alt="X-end Idler" style="width: 600px; align: left;"/>

<img src="img/prusa/broken-x-end-idler05.jpg" alt="X-end Idler" style="width: 600px; align: left;"/>

<img src="img/prusa/broken-x-end-idler06.jpg" alt="X-end Idler" style="width: 600px; align: left;"/>

#### And my repair job

<img src="img/prusa/broken-x-end-idler10.jpg" alt="X-end Idler" style="width: 600px; align: left;"/>

## Duplicate Z-axis part

Z-axis assembly: http://manual.prusa3d.com/Guide/4.+Z-axis+assembly/296?lang=en

Step 2: identifying the parts
http://manual.prusa3d.com/Guide/4.+Z-axis+assembly/296?lang=en#s5014

Prusa also offered me a 20% discount on some filament. Seems like a good idea - so I bought some Extrafil (supposed to be good quality filament)

Strangely enough.. Prusa sent me the filament but *not* the missing parts. I contacted them about the missing parts and they were apologetic, and sent me the missing parts via express mail.

<img src="img/prusa/double-z-axis-bottom-left.jpg" alt="Duplicate Z axis Bottom Left" style="width: 600px; align: left;"/>




## Broken bolts in aluminum frame
### Solutions to fixing broken bolts..

Beginning of January 5-7 in final step..


* drilling out the bolts (they're stainless steel, none of my drilling tools or bits could do it)
* cutting a notch in the bolt head and unscrewing it using a flathead screwdriver (the bolt was in too deeply)
* dissolving the bolt using alum (left two days with a tealit alum solution... no effect)

At this point I figured I had dont everything I could possibly do (and it's been two months since I've been building this kit with still no functional printer).. I contacted Prusa to ask for a replacement frame. As always their customer support was very gracious.. despite all the troubles I've run into building this kit, I still  have high regards for the way they treat their customers.

### New aluminum frame arrived on Jan 13
#### Tapping the frame using an M3 tap (purchased at the local hardware store - it was rather expensive! --- but once you use it, the bolts go into the aluminum easily and secure tightly, a huge difference!)
I posted this recommendation on the instructions page...



## Bed Level Problems...
### Really helpful Prusa MK2S owners facebook page..

### Trying to fix this problem....
* Reassembly of Y-axis to get 'perfect alignment'
* Multiple adjustments of the PINDA probe
* Moving the printer to different surfaces (table tops which may be more flat), and recalibrating the printer afterwards
* reassembling the printbed/Y-axis connection

#### Caliper measurements show a 1mm difference in height between the left and right side of the bed, but the PINDA Z calibration should resolve this? No?
To be honest I'm now really regretting not purchasing the slightly more expensive MK3. A friend of mine purchased the MK3 and had his printer up and working in two days. The y-axis frame seems to be a much better design than on the MK2S - which I have had to repeatedly adjust, to the point of even rebuilding the whole thing.. and I can only assume part of my bed height problems are due to the instability of the Y-axis design. At this point I am ready to give up... if you have any suggestions for solving this problem please help!

After assembling my Prusa MK2S kit I am experiencing a problem with getting even first layers. For some reason, the prints are higher up from the bed on the left than on the right.

Getting the right Z-adjust Level
https://shop.prusa3d.com/forum/prusa-i3-kit-building-calibrating-first-print-main-f6/life-adjust-z-my-way-t2981.html

possibly the y-axis is somehow offkilter (right side higher than the left) ... the pinda is not capable of adjusting for this
https://www.reddit.com/r/3Dprinting/comments/5ximfs/is_the_prusa_i3_mk2_mesh_bed_levelling_not_real/

Video of guy with same issue:
<iframe width="560" height="315" src="https://www.youtube.com/embed/VqgqAyFAb7I" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>


## V2Calibration gcode

The calibration print is 'squished' on the right side and sticks well to the bed. The lines get thinner as they go to the left. The lines on the left are not 'squished' and don't stick to the bed.

Apologies for the image - the filament is grey so it is a bit difficult to see against the print bed.

<img src="img/prusa/bedlevel-v2cal02.jpg" alt="Bed Level Problem" style="width: 800px;"/>

<img src="img/prusa/bedlevel-v2cal03.jpg" alt="Bed Level Problem" style="width: 800px;"/>

## Here is the bottom of the tree frog included print.
The left side of the print is not well-attached to the bed, the right side is printed very nicely on the first layer.

<img src="img/prusa/bedlevel-treefrog.jpg" alt="Bed Level Problem" style="width: 800px;"/>

<img src="img/prusa/bedlevel-part01.jpg" alt="Bed Level Problem" style="width: 800px;"/>




## Attempts at Troubleshooting

### Live-Z Adjust

### Bed Level Adjust

### Rebuilding/Tightening the Frame