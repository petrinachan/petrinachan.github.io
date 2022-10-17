---
layout: post
title: "Assignment 2"
author: "Petrina Chan"
categories: assignments
tags: [assignments]
image: assignment-2.jpg
---

# Assignment 2 - Parametric Modelling with Grasshopper

## Files

[Rhino file (single pieces, 2D)](assets/other/A2/PiecesForPrint.3dm)

[Grasshopper file (single pieces, 2D)](assets/other/A2/PiecesForPrint.3dm)

[Rhino file (3D model)](assets/other/A2/3dModel.3dm)

[Illustrator file](assets/other/A2/GrasshopperFile.gh)


## Learning
I’ll be honest – I left last week’s lecture feeling very lost and quite nervous about the material that we covered. Things that are very numbers and logic oriented are very difficult for me to wrap my head around, and using Grasshopper is no different. 


After not 100% following the in-class demo, the first thing I did before starting anything formal for the assignment was watch through the lecture demo; first without following along just so I could really take in the information presented and why certain actions were taken, then while following.


After I successfully followed the demo, I tried to replicate a similar result without referencing the demo. I kind of got there, and then ran into some questions about making the polar array symmetrical. My questions got answered by TA Jun Chao, and I felt like I understood things a lot better. 


I was confused about why I could only divide by -2 to get the polar array to be symmetrical vs. If I adjusted it by another amount it would get out of whack. I learned about how the line of symmetry has to be centered on both the polar array and the main shape.

<img width="231" alt="Screen Shot 2022-10-12 at 12 25 21 PM" src="https://user-images.githubusercontent.com/115116582/196103769-050a55ec-2b03-4cf1-90e6-c87502cff503.png">

<img width="252" alt="Screen Shot 2022-10-12 at 12 25 38 PM" src="https://user-images.githubusercontent.com/115116582/196103758-2bceeee0-cfde-4ee3-9ab9-4b0959a1f9eb.png">


*Symmetrical vs. wonky array*


After figuring that out, I was able to make a simple circle with slots, and I understood why I was doing the things I was doing. I also discovered, after looking at [Grasshopper documentation](https://grasshopperdocs.com/completeIndex.html) that I could use “Region Difference” to trim and join the slots and shape, which to me was a lot easier!

<img width="484" alt="Screen Shot 2022-10-13 at 8 21 14 PM" src="https://user-images.githubusercontent.com/115116582/196105339-fa5c3086-46ff-4412-be88-4a1160040042.png">
<img width="680" alt="Screen Shot 2022-10-13 at 8 18 36 PM" src="https://user-images.githubusercontent.com/115116582/196104666-82465f41-fe0c-45f4-9117-ff0fdd8c8718.png">

## Making pieces in Rhino & Grasshopper

Now I felt like I could make some simple pieces for the assignment. Since I had some leftover cardboard from the same type of box that I used for Assignment 1, I decided to make pieces that would fit with my first assignment. Because the pieces I made for the first assignment were all square-based, I thought that keeping with the circles for the current pieces would be a nice addition to the ocean scene. 

In addition to the basic circle, I wanted to make something a little more interesting, so I thought about taking circular cut outs from the larger circle to make a sort of wavy shape. I played around a little bit and ended up making a polar array of smaller circles that were cut out from the larger one.

<img width="481" alt="Screen Shot 2022-10-14 at 2 33 46 PM" src="https://user-images.githubusercontent.com/115116582/196105406-d08af21f-a8ac-4304-8c32-496caa1fca01.png">

*Experimenting with cut outs*

Something that still confuses me is the “angle” option for polar arrays. It doesn’t behave as I thought that it would (e.g. the array doesn’t rotate the amount of degrees that is inputted), but after some trial and error I was able to get what seemed like a symmetrical result. 

<img width="246" alt="Screen Shot 2022-10-16 at 11 38 26 PM" src="https://user-images.githubusercontent.com/115116582/196106713-99b704b0-8247-4389-b70b-8521c51f7f82.png">

*Angle of 172 vs. angle of 173 with no other settings changed*


Now that I had the set up for these two shapes, I went back and adjusted the parameters so that they matched the requirements for my cardboard and the dimensions of the pieces from Assignment 1. The slots were adjusted to be 2.4mm wide and 3mm deep. The radius of the circle was adjusted to be 12mm (24mm diameter – since the base squares for A1 were 24mm around). Since the two pieces are based off the same base circle, it was nice that I could just bake it at different points and it would give me the two different pieces.

<img width="1266" alt="Screen Shot 2022-10-13 at 8 50 45 PM" src="https://user-images.githubusercontent.com/115116582/196107504-232fa8d7-68b1-4772-9408-1c6d80f8de56.png">

*Entire Grasshopper definition*


<img width="1405" alt="Screen Shot 2022-10-17 at 12 35 30 AM" src="https://user-images.githubusercontent.com/115116582/196116896-b91d6073-37d0-415f-bf12-5bead349ec0b.png">


*Final pieces*


<img width="480" alt="Screen Shot 2022-10-16 at 10 33 58 PM" src="https://user-images.githubusercontent.com/115116582/196107676-313a5591-7535-4d5b-b864-95ef021f5816.png">

*3D render*


## Exporting
After exporting to an .AI file with the correct scaling, I placed the shapes on a 6”x12” canvas since that is the size of my cardboard panels. Since 32 total pieces fit on one canvas, I would need to cut only one panels total for the assignment

<img width="1029" alt="Screen Shot 2022-10-16 at 11 53 43 PM" src="https://user-images.githubusercontent.com/115116582/196108935-ade3d79b-2b09-4896-9cf9-f3c908526904.png">

## Laser cutting 
Since I am using the same type of cardboard as last time, I used the same settings on the laser cutter: 


Power: 100

Speed: 30

Freq: 10


I ran into an error when I clicked print in Illustrator that said my colorspace was wrong, so I switched from CMYK to RGB and it worked; I didn't know it made a difference for the laser cutter.


When I first tried to cut, the laser cutter ran into an error when I pressed the “play” button; it said “Table error – crash detected”. After working with some of the staff at the Mill, we tried turning off auto focus on the printing preferences and restarting the laser cutter. This fixed everything and the cut worked perfectly.

![IMG_20221016_212302](https://user-images.githubusercontent.com/115116582/196109162-35f1e831-aa7f-4843-b2de-01428ec37c05.jpg)

I fit all my pieces from this assignment together with some of the pieces from last time into a random scene/structure.
![final1](https://user-images.githubusercontent.com/115116582/196111640-0ccb5bf1-83be-4198-9e62-6a0b89f09d89.jpg)![final2](https://user-images.githubusercontent.com/115116582/196111669-8fd2a8a4-568a-4cae-8459-fac89164b8b1.jpg)

[Click here for shake test](assets/other/A2/ShakeTest.mov)
