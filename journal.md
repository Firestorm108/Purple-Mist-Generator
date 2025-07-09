---
title: "Purple Mist Machine"
author: "Sidd"
description: "A corona discharge generator for cool visuals using a 20 stage cockroft walton mulitplier!"
created_at: "2024-7-08"
---

<h1>12 Hours</h1>

<h1>July 8th</h1>

First, I thought of the parts I would need and researched the circuit overall. I watched lots of youtube videos and read lots of things. I ended up going with a 6V DC PSU because the transformer that you'll hear about in a second was originally powered by 4 AA batteries in series, a 6V input and 2KV output transformer that I salvaged from a goodwill UVC wand for the overall input power. I went with ceramic capacitors rated for 5KV and a capacitance of 1nF, diodes rated for 5KV and 200mA. I also went with decently thick wire. After that, I started work on the schematic. It took me a while to really get it down even though it doesn't look like a lot, and I'm pretty proud of my first real PCB that wasn't a breakout board. 

![CleanShot 2025-07-08 at 20 53 54](https://github.com/user-attachments/assets/45ba1f9b-1ca2-46f8-b5e2-08da7f8988ac)

After that, I put the components on the PCB. I spaced them out a lot over a 99mmx99mm board because it needs a ton of insulation to not arc. Also, it'll stay cheap this way with my modular design where I can stack PCBs together, which will be the first time using all FIVE PCBs! Definitely the hardest part about all this was wiring the PCBs in a single layer design. FR4 is not able to handle this high of a voltage between layers and it would for sure arc, so I had to make it single layer. This also means it could be milled by a CNC mill which is pretty cool. The PCB isn't done yet of course, with polishing and silkscreen needing to be added.

![CleanShot 2025-07-08 at 20 54 53](https://github.com/user-attachments/assets/6879fc4b-f74e-403c-be14-7488b8189e1f)

After that, I cleaned up the routing and added some silkscreen.

![CleanShot 2025-07-08 at 22 08 06](https://github.com/user-attachments/assets/6fb3a1f7-a3db-4c3e-8ce1-2e5c4ea186ec)

After that, I added parts such as a fan due to the high ozone generation as a byproduct of corona discharge. This happens because the oxygen molecules literally get ripped apart and bind together to create O3, or ozone. Which is toxic to humans and can cause lung disease, so it's a good idea to blow it away from you into a window.

![CleanShot 2025-07-08 at 22 48 27](https://github.com/user-attachments/assets/86a3bd39-84aa-430d-9ed9-298f404d4b19)
Quick drawing of what I want the CAD to look like.

Basically its a sort of rack with all 5 PCBs stacked in there, with the fan on top and electrode pointing outwards.
The electrode is made of thin copper sheet and very pointy to help initiate the discharge.

I also started on uploading models of the components for the cad!

![CleanShot 2025-07-08 at 23 14 59](https://github.com/user-attachments/assets/1d496eea-6694-4b00-8067-f27cb7e18080)

Then I made a wiring diagram, pretty simple since the main stuff is in the PCB. Mostly for safety reasons (ozone and switch) and power input.

![CleanShot 2025-07-08 at 23 23 44](https://github.com/user-attachments/assets/7502c50c-2f4e-449f-ae51-2fd9abaefaa3)

Total Time Spent: 7 Hours



<h1>July 9th</h1>

The entire morning I grinded out the CAD! I'm loving the look, it'll be printing with glass fiber reinforced PETG due to high insulation needs. There are 5 layers with 4 stages each. The control area on the top has 2 switches (one for overall power, one for fan) due to the fan actually decreasing the amount of corona discharge. However, keeping the fan is crucial because ozone is still very damaging so it will only be turned off for testing purposes. The electrode is also in front of the fan, extremely sharp in order to focus the electric field. I also updated the wiring diagram to have the second switch in.

![CleanShot 2025-07-09 at 12 01 25](https://github.com/user-attachments/assets/80b11388-5154-4d66-bb90-de9c6d553759)

![CleanShot 2025-07-09 at 12 04 38](https://github.com/user-attachments/assets/5a27d76d-f9f5-4a03-8fb1-108e4071dbd5)

Also got a nice render!

![Assembly_2025-Jul-09_07-08-52PM-000_CustomizedView5219160649](https://github.com/user-attachments/assets/666001c1-4bc0-414a-be9f-853b5bd51981)

Finally, I finalized the README, BOM, uploaded the files, and got ready for submission!
Super excited to build this, high voltage is really interesting.

Total Time Spent: 5 Hours
