---
layout: post
title: "Assignment 5.5"
author: "Petrina Chan"
categories: assignments
tags: [assignments]
image: assignment-5-5.jpg
---

# Assignment 5 - Meshes & Lamp p.1

## Files 
[Wall hook from Thingiverse](https://www.thingiverse.com/thing:2027331)


[Parrot from Thingiverse](https://www.thingiverse.com/thing:2020400)


[Parrot hook 3DM](assets/other/A5/parrot hook.3dm)


[Parrot hook STL](assets/other/A5/parrot hook.stl)


[Organic platform STL](assets/other/A5/Platform.stl)


## Meshes
I wanted to make something functional and not just decorative for this assignment. While looking around my apartment for simple things that I used, I noticed the boring command hooks that I have in my entryway. 

While browsing Thingiverse for bird related things (just because I like birds, of course I had to look lol), I realized that I could easily combine a bird that stands upright, like a parrot, with a wall hook. This would work well especially if the bird has a flat back that could be pressed against the wall. 

I found this parrot that is apparently LEGO compatible that I thought would be perfect. It’s kind of low poly looking, which would make it look a bit sleek and minimalistic. 

<img width="716" alt="Screen Shot 2022-11-06 at 1 41 31 AM" src="https://user-images.githubusercontent.com/115116582/200490010-a072c1bf-a5ad-4109-9ec7-a6e1379766fd.png">


Next, I found a hook that would match. I found this two-tiered sort of squared hook that looked like it would fit nicely with the parrot.

<img width="739" alt="Screen Shot 2022-11-07 at 10 43 41 PM" src="https://user-images.githubusercontent.com/115116582/200493520-4f1b5d2a-ed5e-4a2c-9fca-0b25d9abc8bf.png">


When I imported them into Rhino, I noticed that the parrot is tiny compared to the hook. I guess it made sense for it to be small since it is meant to work with LEGO. I scaled the parrot up just by eyeballing what would look appropriate with the hook. At this point I didn’t realize how large the hook was.

<img width="502" alt="Screen Shot 2022-11-07 at 10 50 56 PM" src="https://user-images.githubusercontent.com/115116582/200494641-b7997ae4-7d92-41a7-bc79-a83f9cb9dfe8.png">


After resizing, I checked to see if the meshes were closed or open. I used the properties panel and also MeshRepair to check this. While the hook was already a good, closed mesh, the parrot seemed to be an open mesh. I ran MeshRepair on it, and it cleaned up the errors.

<img width="762" alt="Screen Shot 2022-11-04 at 4 56 34 PM" src="https://user-images.githubusercontent.com/115116582/200496139-bce58ca4-5407-4c30-bfd2-41dbd89d8c7a.png">

<img width="784" alt="Screen Shot 2022-11-04 at 5 11 54 PM" src="https://user-images.githubusercontent.com/115116582/200496180-a14335ce-3c50-4024-acd2-7d2e6c43027a.png">


Next, I put the two pieces together in the positions that I envisioned for the hook. The pieces are both pretty nicely shaped, so they came together pretty nicely already at this point. Once I had the parrot in place, I noticed that there was some excess from the model that was sticking out the other end of the hook. To get rid of this, I used MeshTrim and clicked to remove these bits.

<img width="506" alt="Screen Shot 2022-11-04 at 5 13 22 PM" src="https://user-images.githubusercontent.com/115116582/200491757-29ebf43e-d307-46c8-ac32-8c6e7daabd2d.png">

<img width="501" alt="Screen Shot 2022-11-04 at 5 13 29 PM" src="https://user-images.githubusercontent.com/115116582/200496236-24589f1c-aa94-4a51-924a-dfc5a215762f.png">


I also noticed that the parrot was hollow, which again makes sense because of LEGOs, but I wanted it to be solid when printed. I created a circle and put it over the opening and joined it to the parrot. 

![Screen Shot 2022-11-04 at 5 17 21 PM copy](https://user-images.githubusercontent.com/115116582/200491541-e74e495e-4599-4432-888c-0b535468012c.jpg)


Next, I joined the two objects together and made sure that the resulting object was still a closed mesh. 

Then, I exported it to STL and prepared it in Cura. This is when I realized that it was kind of huge, so I scaled it down 50%.

I turned supports on since I thought that it needed it for the head at least. Everything else I left at my default settings and I printed.

I left the house and let it finish while I was away. I came back to a strange scene on the print bed. The print had finished, but a part of the print had broken off and was hanging off the print? It seemed really odd since even the broken off part was printed seemingly correctly. I could not figure out how this could have happened. 

![IMG_20221105_012825](https://user-images.githubusercontent.com/115116582/200493333-f0a29698-f8b1-426a-8eef-25d78be2d70c.jpg)

I went back into Cura and Rhino to investigate and see if anything was off. I noticed a couple small things that I could tweak, but nothing that I think would have caused problems, let alone the problem that happened. 

Some things that I tweaked:
Changed the angle of the parrot tail so that it sits flat on the bed
Changed supports to triangles to be more efficient
Changed supports to only generate where it touches the bed

I sliced, printed and let this run again. Not sure what the difference was or what changed, but it printed out just fine!

![IMG_20221105_191252](https://user-images.githubusercontent.com/115116582/200491968-9766efe3-bbf0-49f4-a6ed-8c8985135f8f.jpg)

![IMG_20221105_191551](https://user-images.githubusercontent.com/115116582/200491979-ef6dfe6a-4bf3-4104-8a0b-c5c900fbd2aa.jpg)


After seeing that it worked, I wanted to print a white version since I thought that would look better in general and it would fit my apartment more.

![IMG_20221106_001915](https://user-images.githubusercontent.com/115116582/200494105-e3463490-7734-4379-9b60-23d973013c88.jpg)

![IMG_20221106_145413](https://user-images.githubusercontent.com/115116582/200494137-038e6730-0d41-4e2e-899e-2aa47acfabcd.jpg)

I stuck a command strip on the back of him and hung him up!

![IMG_20221106_181832](https://user-images.githubusercontent.com/115116582/200494372-b7ec08b1-95ff-4197-bd38-ac553286de17.jpg)

![IMG_20221106_182058](https://user-images.githubusercontent.com/115116582/200494387-c4e33263-f332-4bac-a985-c052c41dba05.jpg)

## Lamp p.1

I didn't get to printing or making anything directly for my lamp this week, but I did sketch out a plan and practice making the types of shapes and objects in Rhino that I want to print.

There are a few artists that I follow that have made lamps using organic things and shapes such as twigs and leaves. I wanted to do something similar, incorporating something perhaps from nature. I was browsing through pictures of other 3d printed lamp structures and thought that some of them looked sort of bone-like, which I thought was cool. 

Eventually, my idea arose, a fish skeleton lamp! My vision is for the bones and housing to be 3d printed (in pieces, then glued together), and potentially wrapped in a thin paper (like rice paper) so that the light will shine through them.

Looking at the lamp innards, the bulb housing has two holes at the top that look like they could be used to attach the lamp shade. If I made ring with two prongs to stick inside those holes, that might be able to hold and stablize the structure.

![IMG_20221108_115519](https://user-images.githubusercontent.com/115116582/200708710-9d7a6b8a-0d91-4800-8dee-30d202b4f733.jpg)
*Holes in bulb housing*


![lamp draft copy](https://user-images.githubusercontent.com/115116582/200710107-ee0f78f5-7a4e-4324-a3fa-1c345fd1d29e.jpg)
*Lamp plan sketch*

I have the option of making the bones more minimalistic or more realistic in terms of texture. If I went more realistic, I would have to learn how to make the organic little bumps and divets of a bone to give it a more organic look. I searched for some tutorials on how to make organic shapes in Rhino and came across some good ones. [This](https://www.youtube.com/watch?v=iwqPI0kN7u4) is one of the best that I found. 

I wanted to try my hand at make some organic objects, so I played around with a few techniques and printed some of my test models.
I learned about:
 - Making surfaces from curve networks
 - Making surfaces from planar curves
 - Blending surfaces (BlendSrf)
 - DupMeshHoleBoundary (using it to close an open mesh)

I eventually made this blobby pedestal-like thing that I thought might be actually useful for displaying figurines and trinkets. Because I was just experiementing and playing around, I didn't organize my work or document things very well, but here is a glimpse of my chaotic sandbox file


<img width="994" alt="Screen Shot 2022-11-08 at 4 42 55 PM" src="https://user-images.githubusercontent.com/115116582/200708190-d308c88d-76d0-4463-85f9-ca6c5aa44b0b.png">

First, I tried printing a mini version of the pedestal and then a larger one.

![IMG_20221108_114406 copy](https://user-images.githubusercontent.com/115116582/200709455-16019bcd-b514-4973-8d26-5df8f6ad0905.jpg)
*Both pedestals*

![IMG_20221108_163632](https://user-images.githubusercontent.com/115116582/200709491-5f10ea88-aa14-4afa-9be8-8cb51a0e2a04.jpg)
*Large pedestal with figurine*

Npw that I'm more confident making organic solids, I can build my sketleton next week!




