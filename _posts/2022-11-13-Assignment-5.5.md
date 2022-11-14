---
layout: post
title: "Assignment 5.5"
author: "Petrina Chan"
categories: assignments
tags: [assignments]
image: assignment-5-5.jpg
---

# Assignment 5.5 - Lamps p.2 Molding & Casting p.1

## Files
[Lamp - All parts 3DM](assets/other/A5-5/LampParts.3dm)
[Lamp - Ring STL](assets/other/A5-5/Lamp ring adjusted.stl)
[Lamp - Fish bones STL](assets/other/A5-5/FishBones.stl)
[Mold 3DM](assets/other/A5-5/eames molds_duplicate.3dm)
[Mold STL](assets/other/A5-5/eames molds_duplicate.stl)
[Mold - Thingiverse model](https://www.thingiverse.com/thing:237419/makes)


## Lamp p.2

Continuing where I left off last time, it was time for me to start modeling and the parts for my lamp. The first thing that I needed to make was the ring I was going to use to attach my main lamp shade parts to the existing bulb housing.

As a reminder, I wanted to make a ring with prongs that fit into the holes on the top of the bulb housing. 

<img width="551" alt="Screen Shot 2022-11-13 at 9 07 10 PM" src="https://user-images.githubusercontent.com/115116582/201592473-f7611715-2eeb-4564-9e08-10ba62ebf4b8.png">


First, I took measurements of the relevant parts (distance between holes, hole width, hole depth, desired ring diameter & radius). I sized down by .02mm for the hole measurements to account for tolerance noise.

Next, I made my pronged ring in Rhino. Here are the steps I took to make the object:

Make rectangles for the inserted end of the prongs using hole dimensions
1. Extrude up
2. Create arms of the prong using the same dimensions but rotated 90 deg
3. Line up arms and inserts 
4. BooleanUnion
5. Make circle curve for ring 
6. Offset 
7. Extrude
8. Move and place around arms
9. Trim excess arms sticking outside of ring
10. BooleanUnion entire shape


<img width="997" alt="Screen Shot 2022-11-13 at 10 30 28 PM" src="https://user-images.githubusercontent.com/115116582/201590613-1655a279-78b3-43a6-8b4e-c8413ca441c5.png">

This was relatively simple! I printed the ring, and it fit right into the holes exactly how I planned. It was a smooth and snug fit while coming in and out with ease. (Forgot to take a photo of this!)

Next was the challenge of making the fish bones. I ended up deviating a little from the original plan because of impatience, a mistake or two, and lack of time. Instead of having two fish in opposite directions, I printed two of the same fish in the same direction. It still turned out nice!

The fish are made up of 4 types of parts: a head, tail, spine, and ribs. The head and tail seemed like the easiest to make shapes, so I saved those for last. 

The first thing I made was the spine. I wanted some organic “bone-like” variation and nuances in these, so I didn’t just make a smooth tube. Steps for making the spine:

1. Draw curve that I wanted the spine to follow
2. Draw randomly shaped closed curves in general desired thickness, tapering toward the ends
3. Loft (make sure there are no twisted parts — some trials and error required here)

There aren’t many steps, but it took me a while to get everything aligned and looking the way I wanted to. Most of it was tinkering around and trial and error, so I don’t have concrete steps to report on for these tweaks.

![Screen Shot 2022-11-11 at 1 09 36 AM copy](https://user-images.githubusercontent.com/115116582/201591302-30ddb751-118d-45b4-8dae-cdff4a476254.jpg)
*Before and after loft*


Next, I made the ribs:
1. Stack two truncated cones with the large base touching
2. BooleanUnion these cones
3. Make a rib shaped curve
4. Flow along curve (turn on stretch)
5. Scale
6. Copy & paste and scale for different sized ribs
7. Move ribs in place, intersecting with the spine.


<img width="327" alt="Screen Shot 2022-11-11 at 1 11 31 AM" src="https://user-images.githubusercontent.com/115116582/201591513-41113f6a-c6b7-4932-b07a-646d79257b0e.png">

<img width="262" alt="Screen Shot 2022-11-13 at 10 36 20 PM" src="https://user-images.githubusercontent.com/115116582/201591681-d841e89f-1ac3-4e9e-93ee-438512f349de.png">


With the ribs in place, I could make my head and tail. These were relatively simple, made of BooleanUnioned rounded triangles that are extruded. I filleted the edges of the tail and one side of the head to give them a slightly smoother look. I forgot to take progress shots of the process, but here you can see a glimpse through the curve artifacts from making the tail.


<img width="354" alt="Screen Shot 2022-11-13 at 9 29 10 PM" src="https://user-images.githubusercontent.com/115116582/201591705-83bdd69c-e745-4624-b803-7bf482f9b5da.png">


After placing the head and tail in the appropriate places on the spine, this is what the fish looked like in Rhino.

<img width="277" alt="Screen Shot 2022-11-10 at 10 03 13 PM" src="https://user-images.githubusercontent.com/115116582/201591746-ffae89ee-323e-479e-b341-10f761ae2e51.png">


Next was to print the fish, which was kind of intimidating. I knew it would need some crazy supports because of the odd shape and things coming off of it. I remember seeing some images of prints that used supports that were different from the block shaped supports that take a lot of time and filament to print, so I wanted to find out if Cura was able to generate these types of supports. I found out about [tree supports, and that Cura can generate these](https://all3dp.com/2/cura-tree-support/). These supports were hollow and have a unique structure so that they offer appropriate support while supposedly being easier to remove and quicker to print.

So, I brought the fish into Cura and turned on tree supports. It looked so interesting! It really looked like a tree grew around it.

<img width="453" alt="Screen Shot 2022-11-11 at 1 29 09 AM" src="https://user-images.githubusercontent.com/115116582/201592524-4dabbb2f-1a10-40b4-b56e-8527056e0894.png">


<img width="643" alt="Screen Shot 2022-11-10 at 10 02 36 PM" src="https://user-images.githubusercontent.com/115116582/201591783-30d5f8a7-d254-4df5-9b0e-23e53760b766.png">


Print time was ~6 hours. It was quite interesting to watch the support structure build up.

![IMG_20221110_215822](https://user-images.githubusercontent.com/115116582/201591813-f1e56bb4-7060-4e69-9cc8-84735b38c3cc.jpg)

![IMG_20221111_025408 copy](https://user-images.githubusercontent.com/115116582/201591862-ee6d2e44-8884-4e9d-b3fd-90f14e9dbcce.jpg)


When it came time to remove the supports, I ran into some trouble. I broke my print! I was so angry since it was 4am and took 6 hours to print. There was one part of the print that was enclosed in the “tree” and I didn’t realize that and snapped it while pulling the support off. It was in a weird position and couldn’t be easily fixed with glue. Next time, I will be cutting the supports to help get them off. The good thing is that this broken print came in handy. I used it as a reference to measure other pieces later when assembling the lamp. 

![IMG_20221111_034112](https://user-images.githubusercontent.com/115116582/201591845-b3a795c6-c52f-49e8-8115-0d75a1a66e5b.jpg)
* ignore messy floor! *


So after print #2 finished, I took scissors and cutters to more carefully remove the supports, and luckily it did not break. Rinse and repeat with print #3 – This is when I decided to just reuse the same model rather than make a new one in a different orientation for the other fish on the light. (18 hour printing time total for these 3 fish @_@).

![IMG_20221111_202614](https://user-images.githubusercontent.com/115116582/201591921-ed3ab478-b2fd-426f-8100-6718e465fecc.jpg)
*Cutting supports out*

To attach the two fish to the ring, I super glued them and let them dry overnight. I supported them by resting them on duct tape rolls on top of a couple tissue boxes, which worked surprisingly well.

![IMG_20221111_204345](https://user-images.githubusercontent.com/115116582/201591970-bb80dbc0-dd18-4fa9-a3da-5ebb11ffe8db.jpg)


The next day, the fish had dried and seemed sturdy! I was worried that they wouldn’t stick correctly; they did take longer to dry than I thought they would. I tested how they looked like on the light:

![IMG_20221112_131454 copy](https://user-images.githubusercontent.com/115116582/201591993-5ec0a2ab-c46e-4da0-be8d-01c45a7232c2.jpg)


Looked pretty good! For the finishing touch, I needed to add some thin paper to diffuse the light and give the fish a “body” as planned. I picked up this interesting translucent paper that had some cool texture at the art store. I planned to stick it to the fish with some Mod Podge. 

![IMG_20221113_215633](https://user-images.githubusercontent.com/115116582/201592242-5bc5b091-1215-4dbd-b759-d79f4a60ba94.jpg)



Using the broken fish from earlier, I drew out a fish shape on a piece of paper to use as a template. I cut the shapes out of the special paper and glued them to the fish. 


![IMG_20221112_164216 copy](https://user-images.githubusercontent.com/115116582/201592193-bb400b92-d413-44b5-b571-e09de65561be.jpg)

![IMG_20221112_165733](https://user-images.githubusercontent.com/115116582/201592257-bc2ae148-3b46-478f-885d-e5ad3a91379b.jpg)


After letting it dry for a few minutes, the lamp was ready! 


![IMG_20221112_171819 (1)](https://user-images.githubusercontent.com/115116582/201592299-a19a0803-ffb9-4285-bd2e-ea6aacc8d7b7.jpg)

![IMG_20221112_172429 copy](https://user-images.githubusercontent.com/115116582/201592309-f028bb84-1ce0-43d6-b52b-b96856729862.jpg)

![IMG_20221112_173640](https://user-images.githubusercontent.com/115116582/201592319-c086c3ea-0e92-4273-b405-088d132edce9.jpg)


The ring still comes on and off cleanly.

![IMG_20221112_180811 copy](https://user-images.githubusercontent.com/115116582/201592339-eb04e48a-2808-4bff-aea6-e1c40d422cdd.jpg)


I’m pretty happy with the result; even though it was not ideally what I envisioned, it still looks pretty neat. Maybe someday I will re-attempt. : )

## Molding & Casting p.1

The other week, I found this model on Thingiverse of the Eames House Bird. It was already split in half for printing, so I thought it would be nice to make a mold from it. 

![Screen Shot 2022-11-13 at 10 01 54 PM copy](https://user-images.githubusercontent.com/115116582/201592689-c2128ba8-aa23-42ca-bbe7-ee991ec4c596.jpg)


The plan was to put each half into an corresponding “box” (more like a coffin?) with a few keys, a pour hole, and a vent or two. I made one box/half first

To make the box:
1. Make rectangle
2. Offset
3. Extrude high enough to have enough structural support at protruding belly of bird
4. Add a base to the box by extruding the same initial rectangle
5. BooleanUnion

To make the protruding keys:
1. Make truncated cones
2. Place & align on top of box
3. Boolean Union

To make pour hole and vents:
1. Make cylinder
2. Trim in half with rectangular plane
3. Position in place in box
4. Trim excess

<img width="232" alt="Screen Shot 2022-11-11 at 1 52 28 AM" src="https://user-images.githubusercontent.com/115116582/201593510-a8dbda10-6739-4a0e-bc49-12e61d08dfd7.png">

<img width="495" alt="Screen Shot 2022-11-11 at 1 38 04 AM" src="https://user-images.githubusercontent.com/115116582/201593520-1440e85c-4bf1-490b-917b-a86a7580c387.png">


Next, I mirrored the entire box structure and aligned it to the other bird half. Since everything was aligned to the grid, it was easy to line up exactly for the other half.

The difference here is that the keys had to be sunken holes instead of protruding. To make sunken keys:

1. Rotate keys so that the large side is facing upwards
2. Move downward until aligned underneath the surface 
3. BooleanDifference

I also had to extend the base to compensate for the hole depth.

<img width="493" alt="Screen Shot 2022-11-11 at 2 23 39 AM" src="https://user-images.githubusercontent.com/115116582/201593831-46cf6b9b-7516-4673-b3a0-f5689f235545.png">

<img width="501" alt="Screen Shot 2022-11-11 at 2 16 59 AM" src="https://user-images.githubusercontent.com/115116582/201593877-0a19e7d5-21cb-4538-ae26-8836e4dfb0fa.png">


Molds looked good, so I put them in Cura and printed them. I printed with low quality settings to speed up the print, since it was going to take ~9-10 hours. I didn’t mind a bit lower quality for this because I wanted to see the texture on the final product. 

I let this print over night and woke up to some nice half birds!

![IMG_20221112_115740](https://user-images.githubusercontent.com/115116582/201593916-44da0078-2411-4170-9544-9d7a787256d3.jpg)


It was now time to mix my Oomoo up. I gathered the supplies that I could find in my apartment; some plastic cups and disposable cutlery and chopsticks for mixing.

![IMG_20221112_132609](https://user-images.githubusercontent.com/115116582/201593944-53689b62-e070-476b-8e7e-cb6285883fd3.jpg)


I measured out the equal parts of the two components and mixed them together until it was uniform (~3-4 min).

![IMG_20221112_132816c](https://user-images.githubusercontent.com/115116582/201593969-82888b29-05a5-4082-b4c8-2e13f4aff05c.jpg)


I slowly poured the Oomoo into the prints starting at a low point and letting it creep up on its own.

![IMG_20221112_133908](https://user-images.githubusercontent.com/115116582/201593998-7b03ac11-eaf0-449b-86c3-4bd43e36e415.jpg)


![IMG_20221112_134101 copy](https://user-images.githubusercontent.com/115116582/201594004-5f53792a-df85-423f-ace6-7ea1e9e0d74f.jpg)

6 hours later… It was time to release the molds! It was kind of hard to release these, they were really tight in the box! First, I separated all corners and sides with my fingers and actually used the scraper from my 3d printer to help pry them out. I was kind of scared I would damage them, but they came out just fine!

![IMG_20221112_195731](https://user-images.githubusercontent.com/115116582/201594025-6741ede7-8d98-4854-85fd-da9a40e91a8a.jpg)

![IMG_20221112_200245](https://user-images.githubusercontent.com/115116582/201594043-4006a2dc-1f09-4c13-9f34-c47729ecadfc.jpg)

![IMG_20221112_201917](https://user-images.githubusercontent.com/115116582/201594123-de10394b-5896-406a-a893-15820000e84a.jpg)

However, as you can see the pour tube is kind of weird. Oomoo seemed to have seeped underneath the tube, between the cylinder and the rest of the mold.


I realized later that these cylinders weren’t sitting even and flat with the main bird part of the mold which was probably causing this problem. See the space between the half cylinder and the rest of the mold in red below.

![Screen Shot 2022-11-11 at 2 23 39 AM copy](https://user-images.githubusercontent.com/115116582/201594266-18279734-3ad1-4766-9276-e4dabc9934be.jpg)


I ended up trimming off some of the extra flaps on the tube with scissors. It isn’t totally clean, but enough to pour stuff down, I think.


The keys fit together perfectly, and everything was aligned!

![IMG_20221112_201204c](https://user-images.githubusercontent.com/115116582/201594324-4f4c3c93-43b0-460a-a502-453030e2133b.jpg)

![IMG_20221112_201821 copy](https://user-images.githubusercontent.com/115116582/201594658-dff7ab54-4bc2-49ed-a19a-9e24abb4cf33.jpg)

![IMG_20221112_201438](https://user-images.githubusercontent.com/115116582/201594401-124d6bb1-d127-4496-8b2d-e3014543d638.jpg)
*testing structual integrity of deepest parts*

## Credits:
Thigiverse user ibudmen for [Eames Bird model](https://www.thingiverse.com/thing:237419/makes)
[Article on tree supports](https://all3dp.com/2/cura-tree-support/)



