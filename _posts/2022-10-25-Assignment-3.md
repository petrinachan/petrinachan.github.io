---
layout: post
title: "Assignment 3"
author: "Petrina Chan"
categories: assignments
tags: [assignments]
image: assignment-3.jpg
---

# Assignment 3 - Getting started with 3D printing! :tada:  

## Files :file_folder:

### 3DM
[2cm cube](assets/other/A3/3DM/2cmcube.3dm)

[3cm tube](assets/other/A3/3DM/tube.3dm)

[3cm cylinder](assets/other/A3/3DM/Cylinder.3dm)

[Nested birds](assets/other/A3/3DM/nested-1cm.3dm)

### STL
[2cm cube](assets/other/A3/STL/2cmcube.stl)

[3cm tube](assets/other/A3/STL/Tube.stl)

[3cm cylinder, .1mm tolerance](assets/other/A3/STL/Cylinder1mmTol.stl)

[3cm cylinder, .001m tolerance](assets/other/A3/STL/Cylinder001mmTol.stl)

[Nested birds](assets/other/A3/STL/nested-revamp-1cm.stl)

### gCode
[2cm cube, low quality](assets/other/A3/gcode/CE3PRO_2cmcube.gcode)

[2cm cube, standard quality](assets/other/A3/gcode/2cmcube_standardQ.gcode)

[2cm cube, super quality](assets/other/A3/gcode/2cmcube_superQ.gcode)

[2cm cube, standard quality, concentric layers](assets/other/A3/gcode/2cmcube_standardQ_concentric.gcode)

[3cm tube single wall extrusion, 3cm tube double wall extrusion, 3cm cylinder 0.1mm tolerance, 3cm cylinder .001mm tolerance (4 objects)](assets/other/A3/gcode/Cylinder_first4.gcode)

[3cm cylinder, on side w/ supports on](assets/other/A3/gcode/Cylinder_side.gcode)

[3cm cylinder, spiralized outer contour](assets/other/A3/gcode/Cylinder_spiralize.gcode)

[Nested birds](assets/other/A3/gcode/CE3PRO_nested-revamp-1cm.gcode)


## Preface
I scored a great deal on a used Ender 3 Pro off Craigslist! The guy lived just a few blocks away from me and was super nice. He sold me the printer along with a spool of black filament already loaded, a glass bed already attached, in addition to a bunch of tools and odds and ends. 

Since the printer was already all assembled, I didn’t have to put it together from scratch. After finding a nice spot for it in my studio apartment (it sits across the dining table from me), I checked to see that it was still set up well and nothing shifted during moving. 

![IMG_20221025_135124 copy](https://user-images.githubusercontent.com/115116582/197884802-28911514-82e2-4841-920d-6fa99228a804.jpg)
![IMG_20221025_135131](https://user-images.githubusercontent.com/115116582/197892155-88371554-cbf1-41c6-ab33-239d504f6475.jpg)


I didn’t have to adjust anything with the hardware during the initial setup inspection. It looked great! The guy I bought it from also said that he did a test print just the day before to check that everything was working as it should. 

Since I was going to be out of town for a week almost immediately after the class where we would be learning about setting up our printers and printing, I had to get a head start on the assignment since the next time I would see my printer would be late Monday night before the due date. I got all of my prints done, except for the nested object, before the lecture on 3D printing.

## Leveling
Before becoming aware of the CHEP protocol that we were going to use for class, I used the built in bed leveling program on the printer. It is very similar to the CHEP protocol, but has 9 stops instead of 5. I leveled the bed to the point that I could barely slip a piece of printer paper under the extruder and move it around (with significant amount of friction)

![IMG_20221015_181042](https://user-images.githubusercontent.com/115116582/197884956-f7dfafaf-a888-4bc5-9213-bb41c6d08d52.jpg)


When I went through the CHEP protocol, upon running the print code, I saw some variations in the line thicknesses. I did live adjustments and started over several times until I got lines that looked sufficiently even. The adjustments that I made were not that major, and it all went smoothly! At first, I wasn’t sure if I needed to manually preheat, but I soon realized that the printer will preheat everything for you when you start the print. To save time, I guess you could preheat it manually before, but it only takes about 2 minutes anyway. 

![IMG_20221015_182925 copy](https://user-images.githubusercontent.com/115116582/197885354-66e833b4-1566-47ce-9c9f-4db6c8ebde13.jpg)
*Uneven lines (left) and even lines (right)*


## Printing cubes
I’ve never been so excited about a simple plastic cube! It’s crazy how we can just create these things almost out of thin air. There is a TikTok series that someone does called “Would a Pilgrim Think This is Witchcraft?”, and this would definitely be a yes.

I first made my cube in Rhino using the Cube command. I exported to STL with all the default settings. I quickly found that the print quality was a setting determined in Cura.The low quality cube measured in at 19.9mm. This was already well within the 1mm tolerance outlined in the assignment, which felt awesome! The print took about 21 minutes.

![IMG_20221015_190628](https://user-images.githubusercontent.com/115116582/197885606-bb5641a7-dddf-4821-8389-363d4b723493.jpg)
*My first cube*

![IMG_20221019_160754](https://user-images.githubusercontent.com/115116582/197885689-8010d78b-7824-4469-bb30-0ecd2ce826e5.jpg)

Both the standard quality and super cubes measured exactly 20.0mm! The standard cube took about 26 minutes to print while the super took 50 minutes. 

![standard super](https://user-images.githubusercontent.com/115116582/197886031-786a07a1-e465-4311-b18a-ba4223ae2f91.jpg)


Considering the difference in time it took to print the super vs. standard but the same accuracy and precision, I opted to use the standard setting for the rest of my prints.  

Even though I didn’t have any adhesion issues with these cubes, I wanted to test the glue stick out because it seemed interesting. Before printing my concentric cube, I put some glue down on the bed. HOWEVER… I definitely put way too much glue down and after the print was done, I could not scrape off the cube even after the bed cooled all the way!

I started to panic and ran to printing forums and trusty Reddit threads for solutions. One common solution was to cool the bed and object extremely, either by placing the entire bed in the freezer or fridge. I opted to fill a Ziploc bag with ice cubes :snowflake::snowflake::snowflake: and place it on my cube and bed to avoid having to take off the bed and re-level everything. In my panic, I forgot to take any pictures of this debacle. I cleaned off the glue afterward with rubbing alcohol.

After sweating (on my part) and chilling (on the printer), I was finally able to scrape off my concentric layered cube. Before finding this setting in Cura (shoutout to the settings search function), I was really confused about what “a concentric top and bottom layer” could mean for a cube. I was trying to figure out a way that the actual top and bottom layer could be concentric like inside of each other. It was not computing in my head. But when I saw what was being printed it seemed so obvious! It was cool to see the difference in layer structure between the default cube and the concentric one. You can really see the concentric square rings on the top and bottom. This cube also measured 20.0mm.

![IMG_20221019_160953](https://user-images.githubusercontent.com/115116582/197886241-8b71c524-1919-4b4e-89b0-4d827051a573.jpg)

![IMG_20221015_211058](https://user-images.githubusercontent.com/115116582/197886257-5ec570e3-3a05-4873-9ac5-1f2b20436c16.jpg)
*Looking at the cool structural differences*

## Printing tubes & cylinders
Next up were the tubes and cylinders. I first created the tubes in Rhino by using the Tube command. I decided to make the negative space and positive space in my tube the same width. I also created the cylinders using the Cylinder command. 

![IMG_20221025_143459_2](https://user-images.githubusercontent.com/115116582/197886803-d14f0349-55a6-416a-986f-2f93b0663152.jpg)
*Measurements for my tube*

After exporting my tube to STL, I loaded it into Cura and was surprised to see that it looked like a box! So weird… After poking around a little bit online to see what the issue may be, I came across this [guide](https://www.simscale.com/knowledge-base/export-rhino-stl/) which brought my attention to the Polygon Mesh Detailed Options, or STL Mesh Options as they are called in the current version of Rhino that we have. Since the site says that the defaults settings are “coarse, and therefore large surfaces will be low in polygons to reduce the upload size. If the settings make details look too tessellated, then you can use finer settings on specific objects by converting them to a mesh before the export.”, I decided to increase the options one by one and preview the export. I found that changing the maximum angle to 3 made the tube export normally.

<img width="961" alt="Screen Shot 2022-10-16 at 10 15 29 PM" src="https://user-images.githubusercontent.com/115116582/197887329-adedac5a-443b-4d00-b152-acdc6d76f1a2.png">
*Exporting preview without changing settings*

<img width="958" alt="Screen Shot 2022-10-16 at 10 15 06 PM" src="https://user-images.githubusercontent.com/115116582/197887337-cdfb26ea-5aeb-46cb-8b2a-ee2360fea88d.png">
*Exporting preview after changing settings*

Now, with my correct tube, I could start printing!

I realized that I could put a few prints on one job to be more efficient. The objects in this batch were:
1. A tube 3cm in diameter and 3cm high with a single extrusion wall thickness
2. A tube 3cm in diameter and 3cm high with a double extrusion wall thickness and random z-seam alignment
3. A cylinder 3cm in diameter exported with a 0.1mm tolerance
4. A cylinder 3cm in diameter exported with a 0.001mm tolerance

These could all be printed in the same batch since you can adjust these in the per model settings. These 4 objects all printed with no problems. 
<img width="1440" alt="Screen Shot 2022-10-25 at 11 52 13 AM" src="https://user-images.githubusercontent.com/115116582/197887477-51b555fc-e409-4c28-9294-dcdd739b7a72.png">
*Setting per model settings*

<img width="1440" alt="Screen Shot 2022-10-25 at 11 55 07 AM" src="https://user-images.githubusercontent.com/115116582/197887519-669d140d-e0fc-4df5-b1fd-88111a20df81.png">
*Sliced models ready to go*

Total, the batch with 4 objects, 2 tubes and 2 cylinders, took just under 4 hours to complete.
![IMG_20221016_232947](https://user-images.githubusercontent.com/115116582/197888161-cbece2cc-087a-4285-a9f6-7d8e5bcc238a.jpg)
![IMG_20221017_021642](https://user-images.githubusercontent.com/115116582/197888168-50df327e-7f2d-4074-addc-6a8349fba2c9.jpg)

You can immediately see the difference in texture between the two tubes. The random z seam tube has little bumps of the seam scattered around the shape, while the standard tube has one straight seam. They varied (probably negligibly) by size (.01 mm)

![IMG_20221019_160512](https://user-images.githubusercontent.com/115116582/197887689-416e8e61-8919-443f-8b63-fa711e8d96ef.jpg)
![IMG_20221019_155941](https://user-images.githubusercontent.com/115116582/197888049-d6bbf097-c595-41a5-bfc1-acda649cfd66.jpg)

The two cylinders also varied the same amount – 29.8mm for the .1 tolerance cylinder, and 29.9mm for the .001 tolerance cylinder. 
![IMG_20221019_160218](https://user-images.githubusercontent.com/115116582/197888540-5ad50f70-799c-4fec-9fc1-290a1f783910.jpg)


The next two cylinders, the spiralized and sideways supported, had to be printed separately because their designated  settings are global settings that affect all objects in the print. It’s amazing how the program can just determine supports when not too long ago people had to manually program and draw those as part of the model.

I rotated the cylinder by using the rotate tool in Cura and rotating it 90 degrees. I wanted to print this on its own, so I turned on supports in the global print settings. I saw the supports that were generated in the preview, which looked good to go.

<img width="579" alt="Screen Shot 2022-10-25 at 12 18 41 PM" src="https://user-images.githubusercontent.com/115116582/197888602-79d5312e-8db5-4142-8e97-0fb5f37574d6.png">


The print took about 1 hour and the supports came right off with some light pulling. Some nubby bumps were left on the model, but could definitely be sanded down if needed. When measured on the smooth areas, it was exactly 30.0mm in diameter
![IMG_20221017_223747](https://user-images.githubusercontent.com/115116582/197889049-e5f6e761-e78f-408e-92ee-6ad2ba659db0.jpg)
![IMG_20221017_223804](https://user-images.githubusercontent.com/115116582/197889077-e64e765e-ec0e-4f4c-87bb-8ae842678a5e.jpg)
![IMG_20221019_160133](https://user-images.githubusercontent.com/115116582/197889098-ceada836-70c4-4d1c-a89c-af2d77fc2fe9.jpg)

The last cylinder I printed was the one with spiralized outer contour. I searched “spiralize” in the settings search and found it under “Special Modes”. 
<img width="1037" alt="Screen Shot 2022-10-25 at 12 23 20 PM" src="https://user-images.githubusercontent.com/115116582/197889215-f1f600ba-75a2-47a1-ac8c-0011bb656cb5.png">

I turned it on, sliced, and previewed the print. I wasn’t expecting it to be hollow, so I thought something was wrong. I did some poking around on Google and found out that this mode is often used for vases and similar objects, so it makes total sense that the print would be open on top. The setting allows you to print almost any shape with the thickness of a single wall; the pressure is shifted spirally upwards. This means that there are no real layers. Instead, the model is built up slowly by gentle, even movements of the Z-axis. The object is composed of a long and uninterrupted chain of filaments, which is gradually built up on itself.


This print measured at exactly 30.0mm. It reminded me of a film canister.
![IMG_20221018_000357](https://user-images.githubusercontent.com/115116582/197889402-7f0c5271-f6a1-483e-ac35-ee7572b5c0f7.jpg)
![IMG_20221019_155712](https://user-images.githubusercontent.com/115116582/197889409-0722150b-093c-42ee-ba62-495f0100fd67.jpg)
![IMG_20221019_155841](https://user-images.githubusercontent.com/115116582/197889412-86010949-02c1-49c8-b684-0840cd0430a1.jpg)


## Printing Nested Object
The nested object is the one print that I modeled and printed when I got back from my trip on Monday night.

I wanted to make something a little bit more interesting than a box or cylinder, but I didn’t have a lot of time since it was around 12am. I made a simple polyline outline of a bird, nested a smaller bird inside it, and placed a ring around them. :bird::bird:

Here are the steps I followed to make the model:
1. Draw angular polyline curves for the bird
2. Fillet some of the corners to make a nicer bird shape
3. Duplicate the bird and scale it down by 0.4
4. Offset both birds by 0.5cm/5mm (revised to 1cm for final print)
5. Extrude all curves 2 cm
6. BooleanUnion the surfaces that should be connected
7. Make a circle that encompasses the nested birds
8. Repeat the extrusion process with the circle
9. Export to STL

The first time I exported this model and imported it into Cura, I realized that it was way too big, so I scaled it down by 0.7. 

![Screen Shot 2022-10-24 at 8 53 44 PM copy](https://user-images.githubusercontent.com/115116582/197889683-36ca67c1-8d0c-4353-b794-e67939284eed.jpg)
*Original vs. scaled in Cura*

When I printed this, the base layer didn’t adhere to the bed and messed up the print. I thought that maybe the bed somehow became unlevel while I was out of town (building shifting, etc), so I releveled the bed. Oddly, it didn’t really seem like any adjustments needed to be made.

I printed it again, and it got a little further, but eventually detached again and went haywire, though the result actually looks kind of neat.
![IMG_20221024_234049](https://user-images.githubusercontent.com/115116582/197889819-f1e75965-4b75-44c8-9db4-3c6945ce111e.jpg)
*Looks ok....*

![IMG_20221025_001122](https://user-images.githubusercontent.com/115116582/197889852-e931500e-d3af-47d9-8e97-05f06f54ba59.jpg)
*Nevermind*

It was getting really late at this point, around 1am, so I had to figure out a solution that would stick because I couldn’t afford to keep printing and starting over. 

I examined the failed prints and thought that perhaps when I scaled it down in Cura, the thickness of the walls became too thin to structurally support the model as it was building up. I went back to Rhino and remade the model the right smaller size and with an offset of 1cm instead of 0.5cm, so that the walls of the bird and circle were 1cm thick and did not need scaling in Cura.

<img width="473" alt="Screen Shot 2022-10-25 at 1 29 44 PM" src="https://user-images.githubusercontent.com/115116582/197890035-ca19af31-9a19-4473-8ffe-becca8b3fca7.png">
*Rendering in Rhino*

<img width="714" alt="Screen Shot 2022-10-25 at 1 30 08 PM" src="https://user-images.githubusercontent.com/115116582/197890041-37a45b3b-e6dd-40dc-b38a-7158f8ec5493.png">
*Preview in Cura*


I also put a tiny bit of glue down on the bed to ensure more adhesion. I started the print, monitoring it intently for the first half hour. All seemed good, so I did some other work while it was printing.

It was interesting to watch how it filled in the layers from the most inner object to outer.

![IMG_20221025_021252](https://user-images.githubusercontent.com/115116582/197890234-0611de5e-0134-4b27-bd72-375608ece0cf.jpg)
*In progress print*

The print took just over 3 hours and looked perfect (YAY). After letting the bed cool down completely (I left it overnight since it was now around 4am :sleepy:), the prints came right off with a little elbow grease. The birds actually look pretty neat! Some of the measurements varied by .02mm, similar to some of the earlier prints.

![IMG_20221025_112136](https://user-images.githubusercontent.com/115116582/197890290-b299596b-70db-4c1e-ad95-628f0ef7d961.jpg)

![smallbird](https://user-images.githubusercontent.com/115116582/197892878-ff0f2733-a834-4ddf-b954-518913867b47.jpg)
*Small bird measurements*

![bigbird](https://user-images.githubusercontent.com/115116582/197892923-c8bda9ef-21d7-4485-9dc9-7f929755a72a.jpg)
*Large bird measurement*

![ring](https://user-images.githubusercontent.com/115116582/197892947-b5878964-1198-424a-adf2-8fe9dcf3e415.jpg)
*Ring measurements*

![IMG_20221025_112611](https://user-images.githubusercontent.com/115116582/197892392-394a9868-4c54-4046-bc66-f3cc424a3701.jpg)
*Birds on display*

From the measurements of these prints, it looks like my printer prints with about +/- .02mm accuracy, and is rather precise. I forgot to document with photos, but all my cylinders and tubes meausred at exactly 30.0mm height in addition to the widths documented above.

## Credit:
Reddit threads for ice trick for stuck prints [[1]](https://www.reddit.com/r/ender3/comments/mvxy9h/prints_stuck_to_bed_too_well/) [[2]](https://www.reddit.com/r/ender3/comments/hubvbf/ender_3_v2_print_is_sticking_to_bed_to_tightly/)

[Info on spiralize outer contour](https://the3dprinterbee.com/cura-vase-mode-spiralize-outer-contour-basics-settings/)





