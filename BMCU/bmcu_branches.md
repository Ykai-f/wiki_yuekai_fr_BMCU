---
title: BMCU Branches
description: 
published: true
date: 2025-06-04T21:40:04.861Z
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

# New BMCU naming convention
The authors `@4061N` have renamed the version iterations of the BMCUs as follows.


- **BMCU-A** : Version with 130 motors and Photoelectric sensors.
- **BMCU-B** : Version with 370 motors and Photoelectric sensors.
- **BMCU-C** : Version with 370 motors and Hall sensors.
- **BMCU-D** ：BMCU-A integrated with B1 rewind unit. (Updated 25/05/2025)

✅ The Mainboard can be used universally across all versions.
⚠️ The **BMCU-C** requires a new sub-board with Hall sensor.
⚠️ The **BMCU-D** will use the old sub-board (with two photoelectric sensors) and the B1 rewind unit motherboard.

# Current branches of BMCUs

## Branches of the main structure of BMCU

```
BMCU
│
├── BMCU-A : 130 Motor/Photoelectric sensors
│    └── Many 130 Improved version （ Adjustable photoelectric block design, triangular clutch with spring, etc.）
│    └── 130 Steel ball version
│    └── 180 version
│
├── BMCU-B : 370 Motor/Photoelectric sensors
│    └── 370 Original version
│    ├── 370 Steel ball version
│    └── Micro Button Version (Requires a completely different PCB)
│
├── BMCU-C : 370 Motor/Hall Sensor
│    └── Been widly tested to verify its stability and is currently the most recommended version.
│
├── BMCU-D : BMCU-A integrated with B1 rewind unit. (Updated 25/05/2025)
│    └── Very early alpha test.
│
└── CMCU in the future
```

## Branches of the PCB of BMCU
```
BMCU
│
├── Mainboard
│   ├── Default version
│   └── Minor security patch version (small update with enhanced safety)
│
└── Sub-board
    ├── V1 Photoelectric sensors 
    └── V2 Hall sensors

```

### Mainboard

Both versions of the mainboard are universal and can be used for all BMCU versions. 

The difference is that the new version adds more protection to the circuits and reduces the possibility of burning in case of hot-plugging or other accidents (although hot-plugging is still not recommended).

#### Original version
![mainboard_origina_version.png](/assets/images/bmcu_branch/mainboard_origina_version.png =x300)

#### With Enhanced Security Patch

> Some users have reported that **new versions of the mainboard** may have issues, such as unexpected reboots or certain channels malfunctioning despite proper soldering.
>
>The developer is currently working on software-level fixes to address these problems.
>
>If you’d like to try the Hall sensor version, for now you can also try to use the **original version of the mainboard**  with the **Hall sensor sub-board**.
{.is-warning}

![mainboard_enhanced_security_patch.png](/assets/images/bmcu_branch/mainboard_enhanced_security_patch.png =x300)

### Sub-board

#### Original version - Dual photoelectric sensor

![subboard_original_version_1.png](/assets/images/bmcu_branch/subboard_original_version_1.png =x200) ![subboard_original_version_2.png](/assets/images/bmcu_branch/subboard_original_version_2.png =x200) 


#### Hall sensor version

![subboard_hall_sensor.png](/assets/images/bmcu_branch/subboard_hall_sensor.png =x300)


# BMCU-A
## 130 version
![130版本可视图.png](/assets/images/bmcu_branch/130版本可视图.png =x500)
> The model in this picture is the latest version (as of 25/02/2025) of the version 130 model, which in the extruder it uses a Split design and an adjustable photoelectric block (green part) to improve performance.

The original version 130, the most classic and earliest version of the BMCU from the author, has since undergone several iterative updates from the author and other developers to optimise its prints.

The problem with the 130 is that it has a ‘triangular plate clutch’ part, which lacks subsequent durability. It is also prone to various problems during assembly, such as idling gears. But for now, the 130 version is more stable with good fitment

update 31/03/2025 - Since the release of the clutch with springs, the installation and commissioning of the 130 version has been considerably reduced ！

Version 130 is still well used today.

## 180 version
The 180 version is a variant of the 130 version, which uses the 180 motor and has been modified to fit this motor. The rest is still identical to the 130 version, with a triangle plate clutch structure.

# BMCU-B

## 370 version
The 370 version means that its motor uses a `370 motor(24v 6000rpm)` instead of the original FF-130sh motor
![370版本可视图2.png](/assets/images/bmcu_branch/370版本可视图2.png)
  
The 370 version will run theoretically faster, and improves on the original 130 version's potential problems of getting stuck at 99% and feed pressure.
> The 370 version has a different noise aspect than the 130 version, and because the 370 motor has more torque, the BMG gears mesh better, and there is a certain amount of ‘filament chewing’.
{.is-warning}

  
Earlier versions of the 370 had the potential for five-pass explosion. The reason was that when the selected print speed was higher than 100%, the BMCU fed the material faster than the extruder, resulting in abnormal operation. The authors and developers have now improved the situation with a different structure of BMCU, but for now the 370 version is still in beta.

## 370 steel ball version
![bmcu_steel_ball_version.png](/assets/images/bmcu_branch/bmcu_steel_ball_version.png)

The current steel ball version is an excellent version who better solves the problem of photoelectric sensors. It is usually recommended to assemble this version.

# BMCU-C
![hall_version.png](/assets/images/bmcu_branch/hall_version.png)

The Hall version is an upgrade from the steel ball version of the BMCU-B, retaining the mechanism of using a steel ball to detect the presence of consumables and using a Hall sensor to detect the position of the buffer.
This improvement was made to address the problem of five way being poped out that could occur with the original BMCU-B version.

Currently BMCU-C is on test.

# BMCU-D
todo 
https://makerworld.com/zh/models/1447789-bmcu-d-version-130#profileId-1507821


# Should I get a BMCU-A or BMCU-B?


| Feature              | 130/180 Version                           | 370 Version                               |
|----------------------|---------------------------------|----------------------------------|
| **Feeding Mechanism** | Passive feeding; remains quiet and stable as long as there is no resistance in filament feeding. | Active feeding; periodically pushes filament to the printer, which may generate some noise. However, many users report it is still quiet. |
| **Noise Level**       | Generally quieter. Some noise during filament loading and unloading. | Potentially noisier due to active feeding, but user feedback indicates it is still relatively quiet. |
| **Filament Loading/Unloading Speed** | Slower loading and unloading. With some noise. | Very fast loading and unloading but produces noticeable noise. |
| **Assembly Difficulty** | Slightly more complex to assemble. | Easier to assemble. |
| **Maintenance** | Risk of clutch wear over time. | Risk of cleaning of the filament hole. If using metal gears, may generate more black grease residue. |
| **Disadvantages & Issues** | If not installed properly, it may cause the printer to get stuck at 99% after printing, continuously flushing material. | May push up the printer's five-way connector and could cause filament grinding, leading to clogging issues. |
