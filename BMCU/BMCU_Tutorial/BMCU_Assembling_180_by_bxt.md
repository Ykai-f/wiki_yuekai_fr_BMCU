---
title: BMCU Assembling 180 by bxt
description: 
published: true
date: 2025-03-26T12:02:22.844Z
tags: 
editor: markdown
dateCreated: 2025-03-26T11:09:15.871Z
---

# 180 BMCU Assembly Guide


> This content is made by `@白小淘`


#### Materials Preparation (excluding 3D printed parts):

The 180 version is modified from the 130 version, with an identical PCB. For PCB information, please refer to the 130 guide.

Changes in the materials list are minor, so only the differences from the 130 version are noted here. Please check the 130 guide for the full list.

Material changes are as follows:

1. The original `130 motor` is replaced with a `180 motor`. It is recommended to purchase 180 motors with a shaft length of 10mm-12mm. Most 180 motors rated at 12V-24V should work. Recommended link:
   1. PWN17VEE12JA1 https://item.taobao.com/item.htm?_u=qu6u6p3c2bf&id=650572440927&spm=a1z09.2.0.0.7c412e8dH0f2vw Price at the time of writing: 1.8 RMB.
   2. FK-180SH-12280 (significantly increased in price)
2. Buffer spring changed to `0.5 x 6 x 15mm`, quantity: `4`. Purchase link: https://detail.tmall.com/item.htm?_u=qu6u6p36069&id=649882524891&spm=a1z09.2.0.0.4d042e8dhdKyYV&skuId=4728198936063
3. Added clutch spring, specification `0.4 x 3 x 5mm`, quantity: 4. Purchase link: https://detail.tmall.com/item.htm?_u=qu6u6p36069&id=649882524891&skuId=4686949972659&spm=a1z09.2.0.0.4d042e8dhdKyYV
4. `M2x5` countersunk self-tapping screws are used in the 180 assembly guide, quantity: 16. If not purchased, you can use M2x8 from the 130 guide as a substitute.

#### 3D Printed Shell Files:

The shell has been completely redesigned and needs to be fully printed.

Version 1 is only suitable for 180 motors with a full metal shell. If you purchased the recommended PWN17VEE12JA1 motor from the link above, you need to print Version 2.

If you have no specific requirements or don't know the difference between the two versions, please print Version 2.

> Note from Yuekai : Please print version 2.
{.is-success}

Version 1: https://makerworld.com/zh/models/1132822#profileId-1133350

There are two print configurations in Version 1. The first configuration is a complete set of component models, print 4 sets. The second configuration contains only the "Clutch Part B - 4mm Thick 242A", suitable for 4mm 242A gears. The parameter in the 242A gear purchase link shows a 4mm thickness, but the actual received thickness is 3.2mm. If you do get a 4mm 242A gear, use the Clutch Part B from the second configuration.

Version 2: https://makerworld.com/zh/models/1152568#profileId-1156984

> Note from Yuekai : Backup download link [180 version](/assets/files/print_files/180%20version.3mf)

Version 2 updates the appearance and removes some features that block the plastic rear cover of the 180 motor, making it compatible with both full metal and plastic rear cover 180 motors. The print configuration includes a complete component set and an installation aid.

If this is your first time assembling the BMCU, you will also need the base and bracket. Please use the base and bracket files from the group file "BMCU Integrated Package V1.1".

> Note from Yuekai : For the base you can refer to this model, you can choose between the original version base in plate 2 or a newer version base similar to 370 version in plate 6
https://makerworld.com/zh/models/1162813-bmcu-130-version-an-optimized-extruder-search-comb#profileId-1291386

---

#### Component Assembly:

The buffer lengths of the two versions are different. The motor mount of Version 2 is larger than that of Version 1. Other aspects are the same. The tutorial uses Version 2.

1. Take out the bottom cover and insert transparent filament into the LED hole. Cut both ends flush with the surface.
> Text on the picture: Insert the filament flush with the housing

   ![image](/assets/images/build-180/image-20250226183726770.jpg =x350)

2. Fix the filament channel cover to the bottom cover with M2x8 flat head screws.

   ![image](/assets/images/build-180/image-20250226184016509.jpg =x350)

3. Screw the M6 pneumatic connector onto the buffer.

   ![image](/assets/images/build-180/image-20250226184422163.jpg =x350)

4. Place a 0.5x6x15mm spring onto the buffer, then place a 62B bushing. Pinch them together and install onto the bottom cover.

   ![image](/assets/images/build-180/image-20250226184607738.jpg =x350)
   ![image](/assets/images/build-180/image-20250226184618713.jpg =x350)

5. Place a 628 worm gear on the installation aid. Align the motor shaft with the worm gear hole and press down.

   ![image](/assets/images/build-180/image-20250226185717057.jpg =x350)
   ![image](/assets/images/build-180/image-20250226185727169.jpg =x350)

6. Solder 50mm wires to the motor. Pay attention to the direction.

   ![image](/assets/images/build-180/image-20250226185818360.jpg =x350)

7. Mount the entire motor assembly onto the bottom cover.

   ![image](/assets/images/build-180/image-20250226185849036.jpg =x350)

8. Install 4 x 62B bushings onto the bottom cover.

   ![image](/assets/images/build-180/image-20250226191407778.jpg =x350)

9. Assemble two 182A gears with two 2x6mm shafts. Position the gear in the center using the installation aid.

   ![image](/assets/images/build-180/image-20250226191544718.jpg =x350)

10. Assemble one 242A gear with a 2x20mm shaft. Use the installation aid to press in. The thinner step side should be about 6.1mm from the shaft end.

    ![image](/assets/images/build-180/image-20250226191813390.jpg =x350)
    
    Gears ready:
    ![image](/assets/images/build-180/image-20250226191844492.jpg =x350)

11. Insert a 0.4x3x5mm spring into the side hole of Clutch Part B.

    ![image](/assets/images/build-180/image-20250226191945796.jpg =x350)

12. Press the spring with a 3mm tool (a 3mm SL screwdriver shown), then insert the 242A gear into Clutch Part B (larger step down).

    ![image](/assets/images/build-180/image-20250226192109252.jpg =x350)

13. Insert two 182A gears into the other two holes of Clutch Part B. If not centered, insert the shorter side of the shaft.

    ![image](/assets/images/build-180/image-20250226192202684.jpg =x350)

14. Place Clutch Part A and lock with two M2x8 screws. The clutch gears should rotate with spring resistance.

    ![image](/assets/images/build-180/image-20250226192322737.jpg =x350)

15. Insert the clutch assembly into the bottom cover.

    ![image](/assets/images/build-180/image-20250226192441182.jpg =x350)

16. Install two 20082B gears and insert a 2x20mm shaft.

    ![image](/assets/images/build-180/image-20250226192604200.jpg =x350)

17. Assemble the extruder wheel from the BMG parts (screw hole type), two MR85 bearings, and a 5x22mm shaft.
> A word of caution: please handle the combination of BMG gear set, D5*2 shaft and bearings with care, as the fit of the gears and shafts is sometimes very tight, and if it unfortunately gets stuck, it is very difficult to get it out again
{.is-warning}

   - Gather the following parts:  
     - **Extrusion wheel with <font color="red">screw hole</font> !!!!!! IMPORTANT**  
     - **Black set screw**  
     - **One thick axle (5 × 22mm)**  
     - **Two bearings (MR85ZZ)**.
     ![bmcu_installation_2.12.jpg](/assets/images/bmcu_assembly_130_qtbz/bmcu_installation_2.12.jpg =x250)
     
     

then **Assemble the Extrusion Wheel**
   - Assemble as shown in the diagram, paying close attention to orientation.  
   - One end of the **thick axle** must be flush with the bearing (to allow a flat surface for the magnet).  
   - **Don’t forget** to install the black set screw.
   ![bmcu_installation_2.13.jpg](/assets/images/bmcu_assembly_130_qtbz/bmcu_installation_2.13.jpg =x250)

18. Install the extruder wheel into the base and apply grease to all POM gears.

    ![image](/assets/images/build-180/image-20250226195811798.jpg =x350)

19. Install 4 x 62B bushings onto the middle frame.

    ![image](/assets/images/build-180/image-20250226195925212.jpg =x350)

20. Place the middle frame on the base, align all shafts with the bushings.

    ![image](/assets/images/build-180/image-20250226200030982.jpg =x350)

21. Flip the assembly and lock all 5 holes with M2x8 screws.

    ![image](/assets/images/build-180/image-20250226200133363.jpg =x350)

22. Flip back and install the magnet. The magnet should rotate with the extruder wheel.

    ![image](/assets/images/build-180/image-20250226200242179.jpg =x350)

23. Place the PCB onto the middle frame and lock with M2x8 screws.

    ![image](/assets/images/build-180/image-20250226203101663.jpg =x350)

24. Trim the motor wires and solder them onto the PCB.

    ![image](/assets/images/build-180/image-20250226203133549.jpg =x350)

25. Insert two needle bearings into the extruder wheel without screw holes from the BMG kit. Install into the handle, minding the direction.

    ![image](/assets/images/build-180/image-20250226202007817.jpg =x350)

26. Insert the shaft into the handle. After installation, the extruder wheel should spin smoothly.

    ![image](/assets/images/build-180/image-20250226202105818.jpg =x350)

27. Mount the handle onto the assembly. Place a 0.5x6x10mm spring into the middle spring hole.

    ![image](/assets/images/build-180/image-20250226202203793.jpg =x350)

28. Press the handle and insert a 2x6mm shaft from the right side.

    ![image](/assets/images/build-180/image-20250226202344792.jpg =x350)

29. Hold the handle and insert a 2x20mm shaft from the other side until fully seated.

    ![image](/assets/images/build-180/image-20250226202506970.jpg =x350)

30. Finally, install the back cover and lock all 4 M2x8 screws. One module is complete.

    ![image](/assets/images/build-180/image-20250226202616802.jpg =x350)

31. Repeat the same steps for the other three modules. After completion, refer to the 130 guide to test the modules.
