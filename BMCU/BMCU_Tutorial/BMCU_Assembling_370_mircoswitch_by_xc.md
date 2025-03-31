---
title: BMCU_Assembling_370_mircoswitch_by_xc
description: 
published: true
date: 2025-03-26T16:06:17.190Z
tags: 
editor: markdown
dateCreated: 2025-03-26T11:09:20.556Z
---

# 370 Motor Version x BMCU-Stardust Microswitch Modified Version Assembly Guide

> This version is a modified edition by the community member `@星尘`, and the content also comes from him.


## Introduction

1. This guide is for assembling the `370 Version X BMCU-Microswitch Modified Version`, which is highly compatible with the original version but not the BMCU370 original.
2. This means you can also use it as a reference for the original 370 version (non-steel ball inverted version).
3. Project open-source link: [BMCUx - Oshwhub.com](https://oshwhub.com/xingcc1/bmcu-370x)
4. Project model link: [Makerworld CN](https://makerworld.com.cn/zh/models/1000993-bmcu-370-tie-pian-wei-dong-bo-li-zhu-hong-fa-yuan#profileId-1026446) [Makerworld Global](https://makerworld.com/zh/models/1175070-bmcu-370-surface-mount-microswitch-glass-bead-trig#profileId-1184075)
5. For the P1 series, some changes are required such as integrating the five-way connection, which is still under refinement and will be updated later.
6. Feel free to test the firmware (under organization), currently recommended: `BMCU Test Firmware 2-6.bin`.
7. You can customize the firmware and test it here: [bmcu370x github.com](https://github.com/Xing-C/BMCU370x)
8. This project model is based on the BMCU2.5 version shell.

## PCB BOM

1. [【Tencent Doc】BMCU370x - BOM List](https://docs.qq.com/sheet/DTXJPYXVjVXpnY0F3?tab=000001)

## PCB Notes

### Mainboard Soldering Section

1. Pay attention to the diode direction.
   ![potect](/assets/images/build-370x/pcb/potect.jpg  =x350)
- RED : *Default: Not soldered, redundant design*  
- Purple : *Check the diode direction*, there’s another one on the top side

2. Solder the back side as needed.
   ![Myback](/assets/images/build-370x/pcb/Myback.png =x350)
 *For debugging output only, no soldering required*  
- *If you want the mainboard LED on the backside*:  
  - Solder the WS2812 LED on the backside  
  - Bridge to SYS  
- *This area usually doesn’t require soldering*   
   
3. Choose and solder the motor voltage.
   ![motor](/assets/images/build-370x/pcb/motor.png =x350)
- *Motor voltage selection by solder bridge:*  
  - Short **red area** for 12V motor  
  - Short **purple area** for 24V motor  
- *12V step-down circuit area*  
- When using a 24V motor, **the green area is optional to solder**
   
4. Switch the slave part back to dual optocouplers (130 basic version).
   ![motor](/assets/images/build-370x/pcb/light.jpg  =x350)
with this version of PCB we have two options
	1.*Original dual-optical design* (Not recommended, requires bridging the pad on the other side when in use)  
  2.*Recommended:* Use surface-mount micro switch  
- Be careful with the micro switch direction.  
- **Do not press the switch during soldering**, it may deform due to high temperature. Test after cooling.


5. Slave part - Functionality
   ![motor](/assets/images/build-370x/pcb/light_1.jpg  =x350)
**Suggested English:**  
- *Jiali Motor*: Red dot = +; **Other motors are likely reversed** (Red dot = -)  
- *External micro switch* works the same as the surface-mounted one  
- **If using dual optical sensors on the other side**, bridge here. Keep open when using the micro switch.  
- *Test points*: Not used  
- *Buffer indicator LED*: ON for 370 motors, OFF for 130 motors (Color can be changed, green is not recommended)  
- *Filament detection indicator*: Should light up only when filament is present

## Component Assembly

1. There might be some omissions in the tutorial, feel free to point out any mistakes and discuss with fellow members.
2. The shell is photographed based on the first version, so the appearance may vary slightly.
3. Start by assembling the bottom shell.
   ![image-0](/assets/images/build-370x/0.jpg =x350)
4. Install 3 bushings and one MR85ZZ bearing. Ensure the bushings are pressed tightly with tools for the best fit.
   ![image-1](/assets/images/build-370x/1.jpg =x350)
5. Ensure motor wires are soldered properly. If the motor has no worm gear, insert the plastic worm gear aligned with the motor shaft, place it in the bottom shell, align the screw holes, and use M3x5 flathead screws to secure it.
   ![image-2](/assets/images/build-370x/2.jpg =x350)
6. Ensure the glass bead area is smooth. If there are small bumps, trim them with a craft knife.
   ![image-3](/assets/images/build-370x/2.1-new.jpg =x350)
7. After trimming, proceed to the next step.
   ![image-4](/assets/images/build-370x/2.2-new.jpg =x350)
8. Insert two m2x20 shafts. If using metal gears, use 1.95/1.9mm diameter shafts. Also, adjust the bottom shell/mid-frame as metal gears differ in thickness. Metal gears are not recommended.
   ![image-5](/assets/images/build-370x/3.jpg =x350)
9. Press the 182A plastic gear down fully. Align carefully and press the one closer to the motor first. Metal gears can be placed directly.
   ![image-6](/assets/images/build-370x/4.jpg =x350)
10. Take the buffer cylinder printed part and slider, assemble them together. Ensure filament passes through smoothly; otherwise, reprint the cylinder with compensation.
    ![image-7](/assets/images/build-370x/5.jpg =x350)
11. For the new buffer cylinder, insert a spring (diameter 10).
    ![image-8](/assets/images/build-370x/5-new.jpg =x350)
12. Take the BMG gear with a hole, locate the black set screw, a MR85ZZ bearing, and several M5x22 shafts. Test the fit between the shaft and bearing to find the best one that fits easily.
    ![image-9](/assets/images/build-370x/6.jpg =x350)
13. Place the MR85ZZ bearing, insert the selected M5x22 shaft, then fit the BMG gear (smooth side down). Ensure everything is flush, then tighten the set screw with a hex wrench so the BMG rotates with the shaft and bearing.
    ![image-10](/assets/images/build-370x/7.jpg =x350)
14. Add lubricant to the worm gear and 182A gear. Do not lubricate the BMG gear to prevent contaminating the filament.
    ![image-11](/assets/images/build-370x/8.jpg =x350)
15. Ensure proper placement.
    ![image-12](/assets/images/build-370x/9.jpg =x350)
16. Insert the BMG gear carefully, keeping it away from lubricants. The bottom part will get slightly lubricated by contact, but no active lubrication is needed.
    ![image-13](/assets/images/build-370x/10.jpg =x350)
17. Install the buffer and spring. Recommended lengths: 35mm (original), 50mm (extended).
    ![image-14](/assets/images/build-370x/11.jpg =x350)
18. Compress the spring into the shell; prevent it from popping out.
    ![image-15](/assets/images/build-370x/12.jpg =x350)
19. Prepare the middle frame printed part.
    ![image-16](/assets/images/build-370x/13.jpg =x350)
20. Install three bushings on the middle frame; ensure they are as tight as the bottom shell (usually easier).
    ![image-17](/assets/images/build-370x/14.jpg =x350)
21. Prepare for mid-frame installation: route motor wires out evenly without pinching. Align gear shafts with the bushing holes and MR85ZZ bearing with the slot. Ensure the spring stays inside. After securing, test the spring bounce.
    ![image-18](/assets/images/build-370x/15.jpg =x350)
22. Installed look.
    ![image-19](/assets/images/build-370x/15.1.jpg =x350)
23. Carefully flip it over, press to minimize gaps, and fasten with five m2x8 self-tapping screws.
    ![image-20](/assets/images/build-370x/16.jpg =x350)
24. Prepare the lever part: 0.6x4x15 spring (recommended 0.4x4x15), two M2x10 shafts, two ball bearings from BMG package, one shaft, and one BMG gear without a hole (some from 1688 may have holes).
    ![image-21](/assets/images/build-370x/17.jpg =x350)
25. Insert two ball bearings into the BMG gear.
    ![image-22](/assets/images/build-370x/18.jpg =x350)
26. Take the lever printed part (may need sanding if not printed standing) and install the BMG gear with the toothed side facing the thicker side.
    ![image-23](/assets/images/build-370x/19.jpg =x350)
27. Stand it up, press-fit the shaft from the kit, ensuring both sides are in place and centered.
    ![image-24](/assets/images/build-370x/20.jpg =x350)
28. After installation, rotate the BMG gear smoothly. Sand if necessary.
    ![image-25](/assets/images/build-370x/21.jpg =x350)
29. Stand the feeding assembly upright, insert the 0.6x4x15 spring (recommended 0.4x4x15).
    ![image-26](/assets/images/build-370x/22.jpg =x350)
30. Install the lever, aligning the spring with the hole.
    ![image-27](/assets/images/build-370x/23.jpg =x350)
31. Hold the lever and assembly horizontally, align bushing and lever holes for shaft installation.
    ![image-28](/assets/images/build-370x/24.jpg =x350)
32. Insert the M2x10 shaft and press it in with a tool.
    ![image-29](/assets/images/build-370x/25.jpg =x350)
33. Ensure proper installation; the protrusion should not exceed the shell.
    ![image-30](/assets/images/build-370x/26.jpg =x350)
34. Flip to the other side, repeat shaft installation.
    ![image-31](/assets/images/build-370x/27.jpg =x350)
35. Ensure proper installation and prepare for the next step.
    ![image-32](/assets/images/build-370x/27.1.jpg =x350)
36. Prepare a 5mm diameter glass bead (heavier ones like steel balls are not recommended).
    ![image-33](/assets/images/build-370x/28.jpg =x350)
37. Insert the bead into the hole; it should fall freely and drop out if facing down.
    ![image-34](/assets/images/build-370x/29.jpg =x350)
38. Install the radial magnet on the BMG gear shaft (size: 6x2.5mm). Ensure proper clearance with the shell. Do not use ordinary magnets as substitutes.
    ![image-35](/assets/images/build-370x/30.jpg =x350)
39. Place the component PCB.
    ![image-36](/assets/images/build-370x/31.jpg =x350)
40. Secure with two m2x8 self-tapping screws. Tighten after both are in place to prevent PCB tilting.
    ![image-37](/assets/images/build-370x/32.jpg =x350)
41. Solder motor wires with a soldering iron. For old firmware (like 130), distinguish positive/negative to avoid reverse rotation. New firmware (3-14 onwards) auto-detects direction.
    ![image-38](/assets/images/build-370x/33.jpg =x350)
42. Cover with the top plate, ensure no wires are pinched.
    ![image-39](/assets/images/build-370x/34.jpg =x350)
43. Tighten four m2x8 self-tapping screws. Congratulations, you've completed one channel of the assembly!
    ![image-40](/assets/images/build-370x/35.jpg =x350)
