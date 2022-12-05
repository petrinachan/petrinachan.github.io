---
layout: post
title: "Final Project"
author: "Petrina Chan"
categories: assignments
tags: [assignments]
image: final.jpg
---

# Final Project

## Files
[Master 3DM file with all 3D parts](assets/other/final/Heron Components.3dm)
[Illustrator file for laser cutting (side 1)](assets/other/final/HeronSide1.ai)
[Illustrator file for laser cutting (side 2)](assets/other/final/HeronSide2.ai)
[Candle holder from Thingiverse](https://www.thingiverse.com/thing:277712)

### Great Blue Heron Candleholder! 

The end result is fully collapsible into flat parts and easily taken down & put together.
![IMG_1861](https://user-images.githubusercontent.com/115116582/205524261-8ec3e0ac-fe33-4ec2-854c-78b5a8811d15.jpg)
![IMG_20221202_161114](https://user-images.githubusercontent.com/115116582/205524269-11154c73-387c-4374-8b31-09220403afa0.jpg)
![IMG_20221204_135924 copy](https://user-images.githubusercontent.com/115116582/205524796-4393705d-92f5-45f2-bc83-e5629c9cea95.jpg)
![compile 1](https://user-images.githubusercontent.com/115116582/205526119-bddc7473-812d-4860-82c0-7ad5f2bf1ed0.png)
![Combine 2](https://user-images.githubusercontent.com/115116582/205526126-ec34741b-0501-4f60-b627-3c2d5a9c951d.jpg)


## Process
I managed to stay a day or two ahead of schedule throughout the process, which was great! I did not have to fall back on any contingency plans, and was able to basically make the product that I intended to from the start. The process is broken up into key tasks below in the approximate order they were done in.

Approximate timeline in calendar form
<img width="829" alt="Calendar copy" src="https://user-images.githubusercontent.com/115116582/205525002-1858a9a2-b96a-4070-a0ce-2d91b64baf59.png">


### Modeling in Rhino 
Before printing anything, I had to model the parts in Rhino. As outlined in the previous assignment, I had already imported my curves from Illustrator and began making the 3D models. The parts that needed to be made were:


1. Wings x2
2. Tufts on head x2
3. Pegs for connecting x2
4. Mold for platform
5. Candle holder


One change that I made from the initial plan was adding a second connecting peg. I thought this would add sturdiness to the structure, which it did. I planned everything out in 2D and then extruded the appropriate curves for the pieces. 

**Wings:**
1. Extrude curve - 0.25”
2. Extrude 3 decorative lines - 0.25”
3. Position decorative lines half way through wing
4. BooleanDifference to create cutouts
5. Create octagon for pegs based on diameter of outlined circles - 0.4” 
6. Extrude octagon peg - 0.3” (0.05” more than acrylic thickness, since the peg will be going through the hole in the acrylic)
7. Chamfer outside edge 
8. Create cylinder to pierce through center of the peg (eyeballed)
9. Boolean difference to create hollow peg
10. Position peg to sit flush with surface of wing
11. Duplicate peg and position according to other outlined circle
12. BooleanUnion pegs to wing
13. Mirror wing to get appropriate orientation for other side

<img width="948" alt="Screen Shot 2022-12-01 at 11 16 12 PMer" src="https://user-images.githubusercontent.com/115116582/205525043-4476654a-8c12-4f0a-9133-87c4abdb5543.png">


**Tufts:**
1. Extrude curve - 0.25”
2. Create 1 octagon for peg based on diameter of outlined circles - 0.16”
3. Extrude octagon peg - 0.3”
4. Chamfer outside edge 
5. Create cylinder to pierce through center of the peg (eyeballed)
6. Boolean difference to create hollow peg
7. Position peg to sit flush with surface of tuft
8. BooleanUnion peg to tufts
9. Mirror tuft to get appropriate orientation for other side


<img width="393" alt="Screen Shot 2022-12-02 at 12 48 00 AMe" src="https://user-images.githubusercontent.com/115116582/205525050-55846411-201c-4ca8-9110-18e948f8b147.png">

**Connecting pegs: **


1. Create octagon for peg based on diameter of outlined circles - 0.5”
2. Extrude peg - 1.5”
3. Chamfer both ends
4. Create cylinder to pierce through center of the peg (eyeballed)
5. Boolean difference to create hollow peg
6. Duplicate for 2 pegs


![Screen Shot 2022-12-02 at 12 45 12 AM copye](https://user-images.githubusercontent.com/115116582/205525063-b27f4fad-7a7e-4768-a2b6-3692c9e42775.jpg)


After printing, I noticed that the fit was just a little loose (printer printed about .02” too small), so I equally scaled the width and height to compensate for this tolerance noise. The final diameter is 0.52”.

**Mold for platform**


1. Extrude existing platform curve - 0.25”
2. Offset by 0.5”
3. Use extruding offset surveys and surface from planar curves to create mold “box”
4. BooleanUnion all components of mold


<img width="328" alt="Screen Shot 2022-12-02 at 12 48 39 AM" src="https://user-images.githubusercontent.com/115116582/205525144-72963b61-ad82-46d3-a67d-ece81ea5f602.png">


**Candle holder**


I found a candle holder on Thingiverse that I thought would work since it has holes in the body that I can string a wire through. I imported the file and scaled it to my candle dimensions (1.41” diameter, 0.67” high) plus a little wiggle room. 


![Screen Shot 2022-12-02 at 12 46 09 AM2e](https://user-images.githubusercontent.com/115116582/205525152-348557eb-9325-4e7e-8652-9cfae84277a4.jpg)


### 3D Printing 
Since I modeled in inches in Rhino and there is no easy way to change Cura from the metric system, I couldn’t export as STL since STL does not hold unit information. Instead, I learned that I can export as 3mf, which will retain unit information. I exported all of my files as 3mf and imported them into Cura.

The whole printing process took about 2 full days (including overnights), which fit well within my initial plan estimates.

**Wings**
Duration: ~9 hours (ran overnight)
Standard quality, turned ironing on. A little loose, so I just put a layer of tape over the pegs as an effective quick fix. 


![IMG_20221130_113208](https://user-images.githubusercontent.com/115116582/205525193-660dc016-6e56-49eb-a0e6-1110f5a973ff.jpg)


**Tufts**
Duration: ~50min
Standard quality, turned ironing on.
Printed twice because I accidentally broke the pegs off of the first print while playing around with them. Didn’t realize how fragile it is!


![IMG_20221204_140051](https://user-images.githubusercontent.com/115116582/205525363-6eb458fd-e694-4b48-8943-56ee1af98fd7.jpg)


**Connecting pegs**
Duration: ~45mins
Standard quality. Printed twice after increasing size to account for tolerance noise.

![IMG_20221130_225700](https://user-images.githubusercontent.com/115116582/205525268-312e6cc7-2c59-4951-ac49-8d3552cb634b.jpg)


**Candle holder**
Duration: ~2 hours
Standard quality, turned ironing on. No issues.

![IMG_20221204_140113](https://user-images.githubusercontent.com/115116582/205525254-9a4d72e3-ba79-4eba-917c-05470e8da576.jpg)


**Platform mold**
Duration: ~11hr (ran overnight).
Low quality, infill 10%. No issues. 


![IMG_20221201_125926](https://user-images.githubusercontent.com/115116582/205525229-3795d2be-7c47-4f4f-aab4-b0da157db345.jpg)


### Laser cutting
I was actually really nervous about laser cutting because I was reading the manual for the laser cutters at the Mill and it kept saying how flammable acrylic is! I was literally sweating the whole time (but nothing actually went wrong!). 


In my Illustrator file, I have both areas to cut out of the acrylic (the main body of the bird) and areas to engrave (a few decorative lines). The engraving areas are curves that were first outlined with 3pt stroke and then converted to shapes via outline stroke. I’m not actually sure if this makes a difference, but I wanted to make sure there was a distinction between cutting areas and engraving areas, even though I read that the laser cutter only recognizes strokes of .001 as cuts.

I had two files which were mirrors of each other in addition to a test file which was just a cut circle with engraving inside.
I bought 3 12x16” frosted acrylic sheets for this project. Even though I technically only need 2 12x12” sheets, I wanted to make sure that I had some extra material in case I made mistakes.

**Testing**
First, I tested cutting and engraving my test file circle. I selected “Combined” mode so that it would engrave and cut in one go. I used the recommended settings that are provided at the Mill:

Engraving: 90 speed, 60 power, 50 frequency

Cutting: 2 speed, 100 power, 100 frequency

![IMG_20221204_163245](https://user-images.githubusercontent.com/115116582/205525766-56d7d5f5-e17d-4f19-998f-d09d5744b0d6.jpg)


The circle came out great with no issues, so I went on to cut the real pieces.

**The real deal**
I loaded up my files and printed with the same settings that I used for the test prints and they came out near perfectly. 

![IMG_20221130_170906](https://user-images.githubusercontent.com/115116582/205525531-449dbf5b-72f6-4a90-9898-00fa490f949f.jpg)
 
There were some brown burns/soot (?) marks and weird melty/cloudy (?) spots on the edges and just a couple points where I think the acrylic melted a little too much so it wasn’t completely smooth. These were mostly eliminated by cleaning with rubbing alcohol and wet sanding with 600 grit sandpaper. 

![IMG_20221130_173046](https://user-images.githubusercontent.com/115116582/205525503-70982146-afbf-449d-8f8e-f8a8eb91f5b7.jpg)

*Smudgy marks*


![IMG_20221130_173501](https://user-images.githubusercontent.com/115116582/205525843-45312fd0-89cc-4e4d-9e6c-520f7cacbe46.jpg)

![IMG_20221130_225708](https://user-images.githubusercontent.com/115116582/205525851-ba3ac41c-ae75-4dce-b215-fb9993158a8d.jpg)

*Testing parts after cutting*

### Molding and Casting 
Luckily, I had just enough Oomoo to create the silicon mold from my 3D print. If I had extra, I would have liked to make some mini versions of these so that I could use them as auxiliary candle platforms!

The mixing of the Oomoo, pouring, and curing went smoothly, just as it did last time. After ~6 hours, the mold was good to go. 

I used Perfect Cast to make the platform. Because I wanted a little bit of texture on it, I used a rubber spatula to create some waves on the surface of the material. After it cured, I sanded the surface down with 100 and 150 grit sandpaper to create a flat area for the bird to stand on. I had entertained the idea earlier of painting it, but I actually really like the subtle variations it already had and didn’t want to add too much noise and color to the project, so I decided to leave it as is.

![IMG_20221202_142427](https://user-images.githubusercontent.com/115116582/205525907-9a45f16e-c976-4f2d-9eda-8f3581059af3.jpg)


![IMG_20221202_143146](https://user-images.githubusercontent.com/115116582/205525917-3a104467-ed71-448c-92b7-290a9e936130.jpg)

### Finishing Touches & Assembly 

**Painting**

Even though I actually kind of liked how the natural white of the prints looked, I definitely also wanted to see if I liked them colored, as I planned. If I hated it, I could always print another set anyway.

For painting, I bought a can of Krylon Fusion All in One Paint and Primer. I was able to find one in a color really similar to the grey that I originally envisioned. I initially wanted to paint the tufts of hair black, but after seeing how it looked in grey, I decided to keep it. I feel like it is more cohesive and simple with just one color.


![IMG_20221201_133008](https://user-images.githubusercontent.com/115116582/205525991-8a8d5248-128a-437e-9908-43962b555018.jpg)


Since it was pretty cold out (30 degrees), and it would have been a paint to set up outside and the paint can says it works best above 60 degrees, I set up a makeshift station inside my tiny studio apartment. The only place that has both space and ventilation is my stovetop. I turned on all the fans in my apartment and set up a mini fan to funnel stuff up into the hood. It worked…alright? I didn’t feel any effects and hopefully did not get any brain damage.

![IMG_20221201_135210](https://user-images.githubusercontent.com/115116582/205525943-76648c02-fcd2-414d-9f11-2a13abf6e7ae.jpg)


I did several coats on each of the wings and tufts. There were some lumps and bumps because I didn't have a great way to keep everything level while it was drying and I might have put on multiple coats too quickly, but overall it lookedpretty good.

![IMG_20221204_135752](https://user-images.githubusercontent.com/115116582/205526041-5706a6f8-90f9-4734-b1f4-e6336ddbe796.jpg)


![IMG_20221204_135723 copy](https://user-images.githubusercontent.com/115116582/205526044-a5651ff9-a850-425c-89b8-a6e6cacaa6c9.jpg)


**Attaching candle holder**
 
I found some 18 gauge wire at the store that I thought would work well enough for suspending the candle from the bird. It took a little bit of playing around to find a way to string it so that it was both sturdy enough to hold the candle straight, but also didn’t look messy. I ended up weaving through two of the holes in the holder rather than just looping it through one.


![IMG_20221204_135835](https://user-images.githubusercontent.com/115116582/205526063-0e4a4a71-2120-45da-8473-2deec21b3c7e.jpg)


Ideally, I would want the wire to be a little bit straighter with less waves and wiggles from me adjusting it, but I can figure that out another time! 


## Credits:
Kasturi, Jessica Douma, and Emily Rowland for help with laser cutter settings on Slack
[ErikHK on Thingiverse for candle holder model](https://www.thingiverse.com/thing:277712)
