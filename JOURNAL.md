---
title: "Snap Battery Pack"
author: "Siwen Long"
description: "Modular battery pack that can be split like legos"
created_at: "2025-07-06"
---



# 7/7/2025 Started CAD and Ideas
![draft charging attachment design](https://hc-cdn.hel1.your-objectstorage.com/s/v3/d4ff10de8d39f0e77b8c2f7da87a638c0239bd92_batterycharging_draft.png)
![draft charging body design](https://hc-cdn.hel1.your-objectstorage.com/s/v3/3ec57546484d94e42ae56d37d6d4be0b57043e0c_image.png)

Today I started on designing the body and charging ciruit, I'm likely going to be using pogo pins for battery to battery connection but I may use spring contacts for the charging part. After modeling the slide together design, I realized how bulky I would need to make the slides because of 3d printing durability which wouldn't look amazing. I'm considering using magnets and pogo pin combonations, though I'm unsure how strong it would be. I'm also not sure how to make the battery pack extend in more than on direction without additional costs. For wiring simplicity, I want to attach the positive terminal of the battery via wire or some connection next to the bottom so it can be easily connected, but I'm not sure of a good solution other than just running a wire down to it. If I chose to go with the sliding rail design, I would want the button pcb for connections to be a single pcb, though if I decide to do that, I either need to pay for double sided assembly which is expensive or manually solder the pogo pins which seems harder. If I wasn't moving and had my electronics stuff packed away, I would be okay with hand soldering it with my hot air station but I can't easily. Other option is making small pcbs with the pogo pins on them and have them snap off a larger board, fulfilling the minimum size requirements of JLC PCB.



# 7/19/2025 1:44PM PST
![printing of first design](https://hc-cdn.hel1.your-objectstorage.com/s/v3/eab0c445e3594cb4990ff8d8ef3e3afd2dbaaebd_20250719_131859.jpg)
![printing of first design with one module partially out](https://hc-cdn.hel1.your-objectstorage.com/s/v3/d55903fcffbd2f292d6e9801d6d6b155e4ff86e0_20250719_131924.jpg)
So I'm not going to lie, I very much printed this a week ago and didn't do anything on the project :sob:. But yeah the print is kinda mid. Layerlines from 3D printing made the sliding action HORRIBLE to hear; while also not having enough tolerence. On the plus side I was able to measure some dimensional errors so I can design them into my prints next time:

>Snap Battery v1 Sliding mechnisms
Requested Width: 15mm
Actual Width: 15.25mm
Error: 0.25

>Bottom:
Requested Inner spacing: 8.6mm
Actual: 8.3mm
Error: 0.3mm

>Top
Requested Inner spacing: 8.6mm
Actual: 8.4mm
Error: 0.2mm

>Battery
Requested: 19.20 Diameter
Actual width: 18.20mm
Actual length: 18.50mm
Error: 0.7mm~1mm
==Seems like I have to calibrate my dimensional accuracy between X and Y axis==

Isn't that neat? I'm going to use 0.25mm or 0.3mm for tolerances in the future. After figuring out dimensional accuracy things....

I'm probably going to use magnets instead since they will take up less space and would be easier to implement than a 3D printed sliding action.

While looking at similiar designs, I found out Google made a concept for this idea back in 2020!

![Google Pixelbloc](https://media.techeblog.com/images/google-pixelbloc-power-bank.jpg)

It looks like the blocks were connected purely by Usb-c ports, 2 connections between each block which would offer a tight connection but I worry about the durability, what would happen if the port snapped off? The LEDs on the modules seem pretty neat. It looks quite clunky for 2500mah each but maybe they have protection circuits inside the blocks. I do like the IO parts, 2 Usb-A and 1 Usb-C is pretty good in my opinion, or 2 Usb-c and 1 Usb-A.

I think the current goal is to get a system that connects the modules together using magnets. I would want to add possibilities for charging per module, short ciruit protection (probably imporant) but for now I just need them to connect.