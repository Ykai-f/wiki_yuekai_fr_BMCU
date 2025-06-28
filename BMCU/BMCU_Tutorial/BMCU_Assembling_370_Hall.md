---
title: BMCU_Assembling_370_Hall
description: 
published: true
date: 2025-06-28T20:32:05.296Z
tags: 
editor: markdown
dateCreated: 2025-06-17T13:28:36.330Z
---

New version is Still todo
also check https://bmcu.wanzii.cn/doc/build/370hall.html

# BMCU-C (370 Hall Version) Assembly Guide

## Introduction

This guide is written for BMCU-C v0.2 channel component assembly.


## Pre-assembly Preparation

Integration package for this tutorial: Coming soon, please check group files

- **A fully soldered BMCU `Hall version` circuit board**: ensuring no soldering defects (cold joints, missing solder, bridges, wrong components, etc.).
- **Flash the mainboard with Hall version compatible firmware**. As of 23/06/25, the latest available firmware is `Test 0013`
- **3D printed housing** : You can choose between 
	[1. The original file from the author](https://makerworld.com/zh/models/1322913-bmcu-c-hall-sensor-version#profileId-1359453)
  [2. Our optimized version](https://makerworld.com/zh/models/1539594-bmcu-c-v0-2-model-kongming-optimized-final-version#profileId-1615601)
  **I strongly recommend you to use the optimized version!**
- **Print this tool to check the polarity of magnets later** [Magnet Polarity Detector](https://makerworld.com.cn/zh/models/1141340)

![Magnet Polarity Detector](/assets/images/bmcu_c_hall/极性确定装置.jpg =x300)

## Main Content

### Component Names

![Component Names](/assets/images/bmcu_c_hall/名称介绍.jpg =x300)

1. Middle Frame
2. Front Cover
3. Bottom Frame
4. Buffer Slider
5. Filament Detection Slider
6. Nut Plug

### Install Bushing

Insert 62B bushing into back cover and middle frame as shown

![Install Bushing](/assets/images/bmcu_c_hall/轴套.jpg =x300)

### Assemble D2\*20 Shaft with 182A Gear

Ensure both ends protrude approximately equal lengths

![Assemble Shaft and Gear](/assets/images/bmcu_c_hall/齿轮轴.jpg =x300)

### Install Worm Gear on 370 Motor and Solder Wires

Align motor shaft with worm gear. Apply 502 glue if needed.

The pin with red dot is positive

![Install Worm Gear](/assets/images/bmcu_c_hall/蜗杆.jpg =x300)

### Determine Slider Magnet Polarity

> You can use the magnetic pole detection device designed by @Wanzi to detect the magnetic poles of a magnet. 
> [Magnet Polarity Detector - Link Makerworld](https://makerworld.com.cn/zh/models/1141340)
{.is-info}

Find a container and add water

![Water Container](/assets/images/bmcu_c_hall/Magnet_dirction.png =x300)

Attach two D3\*10 magnets or one single D3\*20 magnets, place in the [Magnet Polarity Detector](https://makerworld.com.cn/zh/models/1141340), and float on water

The geographic north pole is slightly different from the geomagnetic north pole, so just take the one with a similar direction.

Once stable, the end pointing south is the south pole, the other end is north pole

### Install Magnet in Slider

With slider oriented as shown, insert magnet with south pole down (south pole near pneumatic fitting location)

![Install Magnet in Slider](/assets/images/bmcu_c_hall/Insert_magnet.png =x300)

Important: **Center the magnet in the slider's magnet mounting position**

### Secure Slider Magnet

Use M2*8 self-tapping screw to secure

![Secure Slider Magnet](/assets/images/bmcu_c_hall/滑块螺丝.jpg =x300)

### Install Motor

Place motor in position and secure with M3*5 machine screw

![Install Motor](/assets/images/bmcu_c_hall/电机螺丝.jpg =x300)

### Install Nut and Nut Plug

Place M3 hex nut in recess and insert nut plug to secure

![Install Nut and Plug](/assets/images/bmcu_c_hall/螺母塞.jpg =x300)

### Install Gear

![Install Gear](/assets/images/bmcu_c_hall/齿轮.jpg =x300)

### Assemble BMG Drive Wheel


These are all the parts included in the BMG gear set:

![BMG Gear Set](/assets/images/build-370/components/BMG齿轮套装.jpg =x300)

Take one **D5x22mm shaft** and two **MR85ZZ bearings**. Press the shaft into one bearing until flush.


> Apply even force during installation. Install the shaft vertically to avoid damaging the bearing. Check shaft precision before use—some may not be perfect.
{.is-warning}


![BMG Drive Gear Step 1 - Bottom Bearing](/assets/images/build-370/components/组装bmg主动轮-1-底部轴承.jpg =x300)
![BMG Drive Gear Step 2 - Bearing In Place](/assets/images/build-370/components/组装bmg主动轮-2-底部轴承安装到位.jpg =x300)

Place the **BMG gear with set screw hole** as shown:

![BMG Drive Gear Step 3 - Insert BMG Gear](/assets/images/build-370/components/组装bmg主动轮-3-bmg.jpg =x300)

Insert the **set screw** using a hex key.

![BMG Drive Gear Step 4 - Set Screw](/assets/images/build-370/components/组装bmg主动轮-4-顶丝.jpg =x300)

Install the **top bearing**, ensuring it sits flush against the gear.

![BMG Drive Gear Step 5 - Top Bearing](/assets/images/build-370/components/组装bmg主动轮-5-顶部轴承.jpg =x300)
![BMG Drive Gear Step 6 - Completed](/assets/images/build-370/components/组装bmg主动轮-6-完成.jpg =x300)

Place the assembled **BMG drive gear** into the back frame, gear facing upward.

![Insert BMG Drive Gear](/assets/images/build-370/components/把bmg主动轮放入后盖.jpg =x300)

### Assemble BMG Driven Wheel

Insert two **needle bearings** into the **Driven gear (no set screw hole)**.

![Driven Gear Step 1 - Insert Needle Bearings](/assets/images/build-370/components/组装bmg从动轮-1-放入滚针轴承.jpg =x350)

Place it into the **lever**, making sure the direction is correct, and insert the shaft from the BMG kit.

![Driven Gear Step 2 - Insert into Lever](/assets/images/build-370/components/组装bmg从动轮-2-放入扳手-插入轴.jpg =x350)

### Install BMG Drive Wheel

![Install BMG Drive Wheel](/assets/images/bmcu_c_hall/bmg.jpg =x300)

### Install Ball Bearings

![Install Ball Bearings](/assets/images/bmcu_c_hall/钢珠.jpg =x300)

### Install Filament Break Slider

Note slider orientation

![Install Filament Break Slider](/assets/images/bmcu_c_hall/断料滑块.jpg =x300)

### Apply Grease

> Here @Wanzi uses lubricant, but please note that we do not recommend the use of lubricant, but rather a grease with a certain viscosity, such as the one supplied with the Bambulab machine.
>
> But also, you should not choose a grease with too high a viscosity, for example, it is not recommended to use a grease for bicycles.
{.is-warning}


Lubricate gears (can remove to apply and reinstall, BMG doesn't need lubrication)

![Lubricate Gears](/assets/images/bmcu_c_hall/润滑齿轮.jpg =x300)

Lubricate slider (optional)

![Lubricate Slider](/assets/images/bmcu_c_hall/润滑滑块.jpg =x300)

### Install Slider and Springs

Place two `0.8*12*25 springs` at slider ends, secured in mounting positions

![Install Slider and Springs](/assets/images/bmcu_c_hall/滑块弹簧.jpg =x300)

### Install Filament Break Slider Spring

Place one `0.3*4*5 spring` above filament break slider

![Install Filament Break Spring](/assets/images/bmcu_c_hall/断料滑块弹簧.jpg =x300)

### Install Middle Frame

Attach middle frame to back cover, ensuring magnet portion of slider passes through

![Install Middle Frame](/assets/images/bmcu_c_hall/中框.jpg =x300)

Secure with five M2*8 self-tapping screws

### Install Lever

> If available, now we recommend 0.6*4*15 springs, currently 10 lengths are considered too weak!
{.is-warning}


Place one ~~`0.6*4*10`~~ `0.6*4*15 spring`in position, then install lever

![Install Lever 1](/assets/images/bmcu_c_hall/扳手1.jpg =x300)

Hold lever and insert D2*20 shaft

![Install Lever 2](/assets/images/bmcu_c_hall/扳手2.jpg =x300)

Press firmly to bottom, then use screwdriver to press into recess

![Install Lever 3](/assets/images/bmcu_c_hall/扳手3.jpg =x300)

### Install Radial Magnet

Attach D6*2.5 radial magnet above BMG drive wheel, ensuring it's not compressed and rotates with BMG (important)

![Install Radial Magnet](/assets/images/bmcu_c_hall/径向磁铁.jpg =x300)


> At this point, insert filament and power motor with 12v~24v to `test filament feeding`, `verify magnet rotation`, and `distribute lubricant`
{.is-info}


### Install Light Guider fiber

Insert 1.5mm fiber optic or simply a transparant PETG filament into small hole next to buffer slider, cut flush, for light guide


### Install Sub-board

Place sub-board in position

![Install Sub-board](/assets/images/bmcu_c_hall/副板.jpg =x300)

Secure with two M2*8 self-tapping screws and solder motor wires

![Secure and Solder](/assets/images/bmcu_c_hall/固定副板并焊接电机线.jpg =x300)

Tuck excess wires here

![Organize Wires](/assets/images/bmcu_c_hall/整理线材.jpg =x300)

### Install Front Cover

Secure with four M2*8 self-tapping screws

![Install Front Cover](/assets/images/bmcu_c_hall/前盖.jpg =x300)

### Install Pneumatic Fitting

Screw pneumatic fitting onto slider

![Install Pneumatic Fitting](/assets/images/bmcu_c_hall/气动接头.jpg =x300)



#### LED Status

> `-` in table indicates no effect on LED or unknown status

| Condition | Side LED | Top LED (Fiber) | Troubleshooting |
| :-------- | :------- | :-------------- | :-------------- |
| No radial magnet | - | Red | Check radial magnet and AS5600 soldering |
| Normal operation | - | Blue | - |
| Channel selected (in use) | - | White | - |
| No filament | Black | - | - |
| Filament loaded | White | - | - |
| Buffer pressed (slider) | Blue | - | If red, reverse slider magnet |
| Buffer pulled out (slider) | Red | - | If LED blue, reverse slider magnet |

Mainboard: Blue for normal printer communication, red for abnormal, any other color indicates malfunction
