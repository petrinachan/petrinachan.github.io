---
layout: post
title: "Assignment 1"
author: "Petrina Chan"
categories: assignments
tags: [assignments]
image: assignment1.jpg
---

# Assignment 1 - Laser Cut Press Fit Construction Kit

## Files

[Rhino file (single pieces, 2D)](assets/other/assignment 1.3dm)

[Rhino file (3D model)](assets/other/assignment 1 3d.3dm)

[Illustrator file (1 cutting page)](assets/other/assignment 1.AI)

## Process

When I was thinking about what I wanted to make for my press kit, I remembered this toy that I played with as a kid:

![ello](https://user-images.githubusercontent.com/115116582/194729941-c5b02011-d456-4fb8-a7fe-fc0b5f491a8e.jpg)

It was a builder kit with different ocean themed components that you could arrange in many different ways. I took inspiration from this kit for my assignment.

I decided to have my kit consist of 2 different parts: waves and fish. These pieces would be able to be fit together in a variety of ways to make different structures and scenes.

Before I did any detailed measuring or model, I made a sketch and a very crude paper prototype of my shapes to check to see if what I was thinking of would work out.

![crudeprotosketch](https://user-images.githubusercontent.com/115116582/194729739-4a737cd9-a6ed-4ee6-afbe-b653a5878b48.jpg)

Since it seemed like the pieces would fit together and the shapes would make sense, I made a more detailed sketch with generic units to be filled in after I take measurements. 

<img width="734" alt="digitalsketch" src="https://user-images.githubusercontent.com/115116582/194729055-c599a328-b60f-4e51-9ca5-09a3ad0a6a8c.png">


Then, I found some cardboard boxes in the recycling to use for cutting. 

I measured the thickness of the cardboard with the calipers (2.4mm). I also tested out a few slot dimensions to see which length would work best for both sturdiness and the design of the shapes in terms of aesthetics and not having part overlap and bump each other. It seemed like 3mm slots would work well. ![calipers](https://user-images.githubusercontent.com/115116582/194730152-0be3b7b0-726d-4020-ace6-d8e49f88d7bc.jpg)


Before getting started in Rhino, I updated the sketch with the proposed dimensions 

[image]

### Making the fish in Rhino: 

<img width="359" alt="fish1" src="https://user-images.githubusercontent.com/115116582/194730202-7dd69e58-6749-4015-a0f6-f8110b140ff7.png">

1. Start with a 24mm square
2. Follow scale in sketch to make the trapezoid tail, slice and join to the body
3. Make a 3mm wide rectangle to create the slots
4. Place rectangles in appropriate spots 
5. Slice, trim, and join to cut out the slots from the fish
6. Fillet the outer corners of the slots

### Making the waves: 

<img width="487" alt="wave1" src="https://user-images.githubusercontent.com/115116582/194730246-31a1eec4-755b-4541-9dc7-03bd88240e41.png">

1. Start with a 24mm x 72mm rectangle
2. Set guidelines at each third (24mm) of the rectangle to guide placement of the wave dips
3. Make 3 angles using polyline tool centered at those guidelines 
4. Fillet the 3 angles to make the rounded wave dip
5. Slice, trim, and join to make a complete wave pieve
6. Take the same 3mm rectangle from the previous shape to create the slots
7. Place rectangles in appropriate spots 
8. Slice, trim, and join to cut out the slots from the wave
9. Fillet the outer corners of the slots

Before finalizing and exporting these curves, I wanted to render the pieces in 3D to see how they would fit together and mockup how the press kit could look like. I extruded the pieces to 2.4mm and built a structure with them. 

<img width="963" alt="3dkit" src="https://user-images.githubusercontent.com/115116582/194730251-e8850fd7-2b44-4563-b676-88cd8ef58879.png">

I colored the pieces in the render, though they will just be cut from plain cardboard. In an ideal world I would like to paint the pieces! 

Next, I exported the file to Adobe Illustrator. Since the laser cutter is in inches and I made my file in mm, I had to specify the scale when exporting.

In Illustrator, I laid out the pieces on a canvas that was the same dimensions as the cardboard pieces I will be cutting on (6” x 12”). I also double checked that the dimensions remained consistent after exporting. Since 10 of each piece fits on each panel, I will cut 3 panels resulting in 30 of each piece.  

<img width="784" alt="illustratorpieces" src="https://user-images.githubusercontent.com/115116582/194730260-cc770bfc-a840-4449-b1a6-aa7da84804fb.png">

Final laser cut pieces to come soon!

Credits:

Jessica Douma for helpful post in Discord about exporting from Rhino to AI
