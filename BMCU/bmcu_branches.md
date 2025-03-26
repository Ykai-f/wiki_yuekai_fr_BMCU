---
title: BMCU Branches
description: 
published: true
date: 2025-03-21T12:54:44.677Z
tags: 
editor: markdown
dateCreated: 2025-02-25T09:43:52.883Z
---

# AMCU / BMCU / CMCU ......
The AMCU is a first generation system, and the project has been discontinued and abandoned.
[AMCU Page1](https://oshwhub.com/an_ye/ams-amcu)
[AMCU Page2](https://github.com/applenana/AP-AMS)



The BMCU is the author's second-generation system, and the author's official development actions will gradually shift to the CMCU once the 370 version has been stabilised.

The CMCU is in the early stages of development by the authors and their team. The CMCU is characterised by closed components similar to the AMS system, and the extruder mechanism will be integrated into a closed dryer box, but with a significant increase in the corresponding DIY cost.


# Current branches of BMCUs
For now, the most classic TTL version and the 130 motor are still standard.
However, due to the scarcity of supply (even in China it is starting to be difficult to buy) and the lack of performance of the 130 motor, the author have shifted his development focus to the 370 version.

~~The author expects to release a printout of the latest version of the 370 in 2 weeks (2 weeks from 25/02/2025)~~
The author's next official release is a steel ball version of the 370, but it's not released yet (updared on 21/03/2025)

As of now, all BMCUs use the same PCB board, but different versions may require different firmware to be flashed.

## Branches of the main structure of BMCU

```
BMCU
│
├── 130 version (Author's most original version)
│    └── Many 130 Improved version （ Adjustable photoelectric block design, triangular clutch with spring, etc.）
│    └── 130 Steel ball version
│    └── 180 version
│
└── 370
│    ├── 370 Original version （Same optoelectronic design as the original 130）
│    ├── 370 Steel ball version
│    └── Micro Button Version (Requires a completely different PCB)
│
└── Next version 370 or CMCU in the future
```
There are a lot of developers releasing their modified versions of 370 at the moment, but iterations of 370 are very fast at the moment.

## Branches of the PCB of BMCU
```
BMCU
│
├── Current BMCU motherboards (no specific version number but generally are this one today)
│    └── Type-C version (Typec interface instead of ttl for flashing)
│
└── Next version PCB BMCU (Design and testing phase, will be updated later）

```
The new version of PCB of BMCU compared with the previous generation of motherboards is now the main new 486 floating ground protection (using pmos), Hall buffer (from the previous generation of digital value buffer to analogue value buffer), this version is not yet stable.




## 130 version
![130版本可视图.png](/assets/images/bmcu_branch/130版本可视图.png =x500)
> The model in this picture is the latest version (as of 25/02/2025) of the version 130 model, which in the extruder it uses a Split design and an adjustable photoelectric block (green part) to improve performance.

The original version 130, the most classic and earliest version of the BMCU from the author, has since undergone several iterative updates from the author and other developers to optimise its prints.

The problem with the 130 is that it has a ‘triangular plate clutch’ part, which lacks subsequent durability. It is also prone to various problems during assembly, such as idling gears. But for now, the 130 version is more stable with good fitment

But version 130 is still the most used version today.

## Type-c version
[The original Type-c version page on JLC](https://oshwhub.com/bilibili233/bmcu0000)
This TYPEC version is a small branch of the BMCU main-board, which cancels the original TTL serial and uses the TYPEC interface to burn firmware.

The type-c version was developed by developer `yhr233` based on the author's original motherboard. Reduced complexity of writing firmware, no longer need a serial converter and the need to press a button to burn the program.

## 180 version
The 180 version is a variant of the 130 version, which uses the 180 motor and has been modified to fit this motor. The rest is still identical to the 130 version, with a triangle plate clutch structure.

## 370 version
The 370 version means that its motor uses a `370 motor(24v 6000rpm)` instead of the original FF-130sh motor
![370版本可视图2.png](/assets/images/bmcu_branch/370版本可视图2.png)
  
The 370 version will run theoretically faster, and improves on the original 130 version's potential problems of getting stuck at 99% and feed pressure.
> The 370 version has a different noise aspect than the 130 version, and because the 370 motor has more torque, the BMG gears mesh better, and there is a certain amount of ‘filament chewing’.
{.is-warning}

  
Earlier versions of the 370 had the potential for five-pass explosion. The reason was that when the selected print speed was higher than 100%, the BMCU fed the material faster than the extruder, resulting in abnormal operation. The authors and developers have now improved the situation with a different structure of BMCU, but for now the 370 version is still in beta.

> Author's opinion: For the 370 version, metal gears do not offer better conditions than plastic gears in terms of durability and ease of assembly.

## 370 steel ball version
![bmcu_steel_ball_version.png](/assets/images/bmcu_branch/bmcu_steel_ball_version.png)

The steel ball version is a future offshoot of the 370 version, which should improve the original structure.

The principle is that when the filaments enter the extruder, the steel ball is lifted up, driving the slider to block the photoelectric detection interface, thereby sending the existence of filaments to the printer.

# Should I get a 130/180 or 370?


| Feature              | 130/180 Version                           | 370 Version                               |
|----------------------|---------------------------------|----------------------------------|
| **Feeding Mechanism** | Passive feeding; remains quiet and stable as long as there is no resistance in filament feeding. | Active feeding; periodically pushes filament to the printer, which may generate some noise. However, many users report it is still quiet. |
| **Noise Level**       | Generally quieter. Some noise during filament loading and unloading. | Potentially noisier due to active feeding, but user feedback indicates it is still relatively quiet. |
| **Filament Loading/Unloading Speed** | Slower loading and unloading. With some noise. | Very fast loading and unloading but produces noticeable noise. |
| **Assembly Difficulty** | Slightly more complex to assemble. | Easier to assemble. |
| **Maintenance** | Risk of clutch wear over time. | Risk of cleaning of the filament hole. If using metal gears, may generate more black grease residue. |
| **Disadvantages & Issues** | If not installed properly, it may cause the printer to get stuck at 99% after printing, continuously flushing material. | May push up the printer's five-way connector and could cause filament grinding, leading to clogging issues. |
