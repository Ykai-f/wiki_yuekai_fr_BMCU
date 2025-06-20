Still todo

# BMCU-C (370 Hall Version) Assembly Guide

## Introduction

This guide is written for BMCU-C v0.2 channel component assembly.


## Pre-assembly Preparation

Integration package for this tutorial: Coming soon, please check group files

- A fully soldered BMCU `Hall version` circuit board, ensuring no soldering defects (cold joints, missing solder, bridges, wrong components, etc.). Firmware flashing tutorial is temporarily available in group files.
- Flash the mainboard with Hall version compatible firmware. As of 25.4.16, the latest available firmware is `0013`
- 3D printed housing
- 3D printed [Magnet Polarity Detector](https://makerworld.com.cn/zh/models/1141340)

![Magnet Polarity Detector](/assets/images/bmcu_c_hall/极性确定装置.jpg)

## Main Content

### Component Names

![Component Names](/assets/images/bmcu_c_hall/名称介绍.jpg)

### Install Bushing

Insert 62B bushing into back cover and middle frame as shown

![Install Bushing](/assets/images/bmcu_c_hall/轴套.jpg)

### Assemble D2*20 Shaft with 182A Gear

Ensure both ends protrude approximately equal lengths

![Assemble Shaft and Gear](/assets/images/bmcu_c_hall/齿轮轴.jpg)

### Install Worm Gear on 370 Motor and Solder Wires

Align motor shaft with worm gear. Apply 502 glue if needed.

The pin with red dot is positive

![Install Worm Gear](/assets/images/bmcu_c_hall/蜗杆.jpg)

### Determine Slider Magnet Polarity

::: tip
While there are many ways to determine magnetic polarity, we recommend using the [Magnet Polarity Detector](https://makerworld.com.cn/zh/models/1141340)
:::

Find a container (bowl, plate, etc.) and add water

![Water Container](/assets/images/bmcu_c_hall/水.jpg)

Attach two D3*10 magnets together, place in the [Magnet Polarity Detector](https://makerworld.com.cn/zh/models/1141340), and float on water

![Magnet Polarity](/assets/images/bmcu_c_hall/磁铁极性.jpg)

Once stable, the end pointing south is the south pole, the other end is north pole

### Install Magnet in Slider

With slider oriented as shown, insert magnet with south pole down (south pole near pneumatic fitting location)

![Install Magnet in Slider](/assets/images/bmcu_c_hall/滑块磁铁.jpg)

Important: **Center the magnet in the slider's magnet mounting position**

### Secure Slider Magnet

Use M2*8 self-tapping screw to secure

![Secure Slider Magnet](/assets/images/bmcu_c_hall/滑块螺丝.jpg)

### Install Motor

Place motor in position and secure with M3*5 machine screw

![Install Motor](/assets/images/bmcu_c_hall/电机螺丝.jpg)

### Install Nut and Nut Plug

Place M3 hex nut in recess and insert nut plug to secure

![Install Nut and Plug](/assets/images/bmcu_c_hall/螺母塞.jpg)

### Install Gear

![Install Gear](/assets/images/bmcu_c_hall/齿轮.jpg)

### Assemble BMG Drive Wheel

Refer to 370 ball bearing version tutorial [relevant section](./370#安装bmg主动轮)

### Assemble BMG Driven Wheel

Refer to 370 ball bearing version tutorial [relevant section](./370#组装bmg从动轮)

### Install BMG Drive Wheel

![Install BMG Drive Wheel](/assets/images/bmcu_c_hall/bmg.jpg)

### Install Ball Bearings

![Install Ball Bearings](/assets/images/bmcu_c_hall/钢珠.jpg)

### Install Filament Break Slider

Note slider orientation

![Install Filament Break Slider](/assets/images/bmcu_c_hall/断料滑块.jpg)

### Apply Lubrication

Lubricate gears (can remove to apply and reinstall, BMG doesn't need lubrication)

![Lubricate Gears](/assets/images/bmcu_c_hall/润滑齿轮.jpg)

Lubricate slider (optional)

![Lubricate Slider](/assets/images/bmcu_c_hall/润滑滑块.jpg)

### Install Slider and Springs

Place two `0.8*12*25 springs` at slider ends, secured in mounting positions

![Install Slider and Springs](/assets/images/bmcu_c_hall/滑块弹簧.jpg)

### Install Filament Break Slider Spring

Place one `0.3*4*5 spring` above filament break slider

![Install Filament Break Spring](/assets/images/bmcu_c_hall/断料滑块弹簧.jpg)

### Install Middle Frame

Attach middle frame to back cover, ensuring magnet portion of slider passes through

![Install Middle Frame](/assets/images/bmcu_c_hall/中框.jpg)

Secure with five M2*8 self-tapping screws

### Install Lever

Place one `0.6*4*10 spring` in position, then install lever

![Install Lever 1](/assets/images/bmcu_c_hall/扳手1.jpg)

::: tip
If your tubing and spool resistance is high, or you use a P1 printer, use [this model](https://makerworld.com.cn/zh/models/1167775) in the lever spring groove to increase grip
:::

Hold lever and insert D2*20 shaft

![Install Lever 2](/assets/images/bmcu_c_hall/扳手2.jpg)

Press firmly to bottom, then use screwdriver to press into recess

![Install Lever 3](/assets/images/bmcu_c_hall/扳手3.jpg)

### Install Radial Magnet

Attach D6*2.5 radial magnet above BMG drive wheel, ensuring it's not compressed and rotates with BMG (important)

![Install Radial Magnet](/assets/images/bmcu_c_hall/径向磁铁.jpg)

::: info Recommendation
At this point, insert filament and power motor with 12v~24v to `test filament feeding`, `verify magnet rotation`, and `distribute lubricant`
:::

::: tip
Insert fiber optic into small hole next to buffer slider, cut flush, for light guide
:::

### Install Sub-board

Place sub-board in position

![Install Sub-board](/assets/images/bmcu_c_hall/副板.jpg)

Secure with two M2*8 self-tapping screws and solder motor wires

![Secure and Solder](/assets/images/bmcu_c_hall/固定副板并焊接电机线.jpg)

Tuck excess wires here

![Organize Wires](/assets/images/bmcu_c_hall/整理线材.jpg)

### Install Front Cover

Secure with four M2*8 self-tapping screws

![Install Front Cover](/assets/images/bmcu_c_hall/前盖.jpg)

### Install Pneumatic Fitting

Screw pneumatic fitting onto slider

![Install Pneumatic Fitting](/assets/images/bmcu_c_hall/气动接头.jpg)

### Completion

You can now connect to mainboard for basic feed/retract testing

If 4020 WS2812B LEDs don't light up, check soldering orientation

![Side-mounted 2812 Diagram](/assets/prepare/侧贴2812.jpg)

#### LED Status

> `-` in table indicates no effect on LED or unknown status

| Condition | Side LED | Top LED (Fiber) | Troubleshooting |
| :-------- | :------- | :-------------- | :-------------- |
| No radial magnet | - | Red | Check radial magnet and AS5600 soldering |
| Normal operation | - | Blue | - |
| Channel selected (in use) | - | White | - |
| No filament | Black | - | - |
| Filament loaded | White | - | - |
| Buffer pressed (slider) | Blue | - | If side LED red, reverse slider magnet |
| Buffer released (slider) | Red | - | If side LED blue, reverse slider magnet |

Mainboard: Blue for normal printer communication, red for abnormal, any other color indicates malfunction
