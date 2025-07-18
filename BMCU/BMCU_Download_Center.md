---
title: BMCU Download Center
description: 
published: true
date: 2025-07-18T21:45:53.016Z
tags: 
editor: markdown
dateCreated: 2025-01-28T14:08:05.158Z
---

# PCB files

## PCB project file
Use EasyEDA to open .epro file

| Version          | .epro                                                                                  | Altium                                                                               |
| ---------------- | -------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Original version | ---                                                                                    | ---                                                                                  |
| Hall version     | [PBMCU_C_Hall.epro](/assets/files/download_center/pcb_files/project/PBMCU_C_Hall.epro) | [PBMCU_C_Hall.zip](/assets/files/download_center/pcb_files/project/PBMCU_C_Hall.zip) |

## Mainboard


> **For Mainboard with Enhanced Security Patch**
> We have noticed that this mainboard may exhibit some abnormal behavior. 
> This could lead to unexpected reboots or even damage the 24V to 3.3V power conversion circuit. 
> Our preliminary findings suggest that the issue may originate from the  **SS54 diode** located at position D4 in the upper-right corner of the board. 
> If you plan to produce this board, we recommend not soldering this diode. Instead, directly bridge the pads using copper wire, solder, or a resettable fuse.
{.is-warning}

> **For Mainboard with Enhanced Security Patch**
> The small diode next to the 75176 chip is modeled in the wrong orientation in the soldering aid, please refer to the silkscreen on the mainboard。
{.is-danger}


| Version                                    | PCB manufacturing files                                                                                                                      | Soldering aids                                                                                                                                       |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Mainboard Original Version**             | [pcb_gerber_main_board_v0.4.zip](/assets/files/download_center/pcb_files/pcb_gerber_main_board_v0.4.zip)                                     | [soldering_aids_mainboard_v0.4.rar](/assets/files/download_center/pcb_files/soldering_aids_mainboard_v0.4.rar)                                       |
| **Mainboard with Enhanced Security Patch** | [pcb_gerber_mainboard_enhanced_security_patch.zip](/assets/files/download_center/pcb_files/pcb_gerber_mainboard_enhanced_security_patch.zip) | [soldering_aids_mainboard_enhanced_security_patch.rar](/assets/files/download_center/pcb_files/soldering_aids_mainboard_enhanced_security_patch.rar) |  |

## Extruder (sub-board)

| version                 | PCB manufacturing files                                                                                | Soldering aids                                                                                                                         |
| ----------------------- | ------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
| **Original version**    | [pcb_gerber_sub_board_v2_2.zip](/assets/files/download_center/pcb_files/pcb_gerber_sub_board_v2_2.zip) | [soldering_aids_sub_board_original_version.rar](/assets/files/download_center/pcb_files/soldering_aids_sub_board_original_version.rar) |
| **Hall sensor Version** | [pcb_gerber_sub_board_hall.zip](/assets/files/download_center/pcb_files/pcb_gerber_sub_board_hall.zip) | [soldering_aids_sub_board_hall.rar](/assets/files/download_center/pcb_files/soldering_aids_sub_board_hall.rar)                         |


# Firmwares

## Recommended firmware
- **BMCU-A** : V0.2 [firmwarev0.2.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_v0.2.zip)
- **BMCU-B** : V3.14 [bmcu_firmware_3_14.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3_14.zip)
- **BMCU-C** : V0020 **(highly recommended)** [BMCU-C-V0.1-0020.zip](/assets/files/download_center/firmware_and_source_code/BMCU-C-V0.1-0020.zip) 
or Noise-Color-Heat Improved version  [0013-Plus-Color-Noise-Heat-Improve.zip](/assets/files/download_center/firmware_and_source_code/0013-Plus-Color-Noise-Heat-Improve.zip)

## For P/X user

- **BMCU-C** : V0020 **(highly recommended)** [BMCU-C-V0.1-0020.zip](/assets/files/download_center/firmware_and_source_code/BMCU-C-V0.1-0020.zip)
Please read carefully the README in the zip file.

<details>
  <summary>Click to view the README.md for P/X user</summary>
  
# 📂 BMCU-C Firmware v0020

This folder contains the **v0020 universal firmware** for **all BMCU-C boards**, including the upcoming dual microswitch Hall sensor version.

> 🔧 "**Universal**" means it works across all A1/P1/X1 printers, as long as you’re using a **370 motor and Hall-based buffer**.  
> The choice of sub-board does not matter; for P1, just ensure the pipe length is configured correctly to choose **internal** or **external** version.  
> A1 is configured as internal by default and does not require adjustment.

---

## 🔤 Firmware Naming (A/B/C/D)

The files named `BMCU-C-0020-P-X-Series-Int/Ext-Hub-A/B/C/D` are specifically for **P1 series**:

- Choose `Int` or `Ext` version according to your Hub location.
- The suffix `A`, `B`, `C`, `D` determines the printer’s ability to recognize up to 4 devices.
- For A1, you can **directly flash `BMCU-C-0020-A Series Printer.bin`** without concern.

---

## 🔧 Practical Examples

Here are some common usage scenarios and the corresponding firmware to flash:

- 🟢 **For A1 mini**:  
  Flash `BMCU-C-0020-A Series Printer.bin`

- 🟢 **For A1**:  
  Flash `BMCU-C-0020-A Series Printer.bin`

- 🟢 **For P1S using a single BMCU with external 5-way hub**:  
  Flash `BMCU-C-0020-P-X-Series-Ext-Hub-A.bin`

- 🟢 **For P1S using two BMCUs with external 5-way hubs**:  
  - Flash `BMCU-C-0020-P-X-Series-Ext-Hub-A.bin` on BMCU #1  
  - Flash `BMCU-C-0020-P-X-Series-Ext-Hub-B.bin` on BMCU #2


## 🗓️ Firmware Update – July 25, 2025 (v0020)

**BMCU-C v0020 Changelog:**

- 🛠️ Fixed incorrect LED behavior where some statuses failed to light up
- ⚙️ Resolved issue with unexpected channel online status
- 🔧 Corrected anti-disconnection mechanism (previously ineffective)
- 💡 Completely reworked the LED system:
  - Fixed flickering issues
  - Reduced LED refresh rate to improve performance
- 🔁 When a channel error is detected, the system now retries lighting up the red LED every 3 seconds.  
  This ensures that channels inserted **after** the BMCU has entered working state will still be detected visually.


**BMCU-C v0019 Changelog:**

- ✅ **16-color support** for P1/X1 printers (requires flashing the new firmware)
- 🛠️ Fixed the issue where **filament info could not be saved** on the latest P1 firmware (`00.01.06.62`) and slicing software (`2.1.1.52`)
- ⚙️ Refined online channel logic to prevent incorrect status detection in edge cases
- ⚡ Improved motor control: separate logic for high and low voltage scenarios

---

## 💡 Changes Compared to Previous v0013 (Anti-Overheat Light Optimization)

- 🌙 Mainboard LED Behavior:
  - Red breathing light when not connected to printer
  - White breathing light when working normally
- 🔅 Further reduced LED brightness for buffer and mainboard to prevent overheating
- 🔁 Ejection behavior revised: removed A1-specific retraction control for broader compatibility

---

If you have any questions or suggestions, feel free to reach out to the community or our support group.  
We’re committed to continuously improving the BMCU firmware experience.

---
  
  </details>
  
## All releases and update log

<details>
  <summary>Click to view all releases</summary>

#### Firmwares for BMCU-A
| Version | Firmware                                                                                          | Note                          | Src |
| ------- | ------------------------------------------------------------------------------------------------- | ----------------------------- | --- |
| V0.2    | [firmwarev0.2.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_v0.2.zip) | ⭐⭐⭐Recommended for **BMCU-A** |[src-bmcu-0-2.zip](/assets/files/download_center/firmware_and_source_code/src-bmcu-0-2.zip)|



#### Firmwares for BMCU-B
Firmware from this version onwards is adapted to the BMCU-B aka 370 version aka,
also starting to support the P-Series recognising the BMCU as an AMS system. 
| Version | Firmware                                                                                                    | Note                                          | Src                                                                                           |
| ------- | ----------------------------------------------------------------------------------------------------------- | --------------------------------------------- | --------------------------------------------------------------------------------------------- |
| 1.21.2  | [bmcu_firmware_1_21_2.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_1_21_2.zip) |                                               |
| 1.26    | [bmcu_firmware_1_26.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_1_26.zip)     |                                               |
| 2.06    | [bmcu_firmware_2_06.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_2_06.zip)     | For 370                                       |
| 2.22    | [bmcu_firmware_2_22.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_2_22.zip)     |                                               |
| 3.14    | [bmcu_firmware_3_14.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3_14.zip)     | ⭐⭐⭐Recommended for **BMCU-B** aka 370 version | [src-bmcu-3-14.zip](/assets/files/download_center/firmware_and_source_code/src-bmcu-3-14.zip) |
| 3.31    | [bmcu_firmware_3_31.rar](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3_31.rar)     |                                               |

#### Firmware for BMCU-C
Firmware from this version adapted to BMCU-C

| Version | Firmware                                                                                                        | Note | Src                                                                                               |
| ------- | --------------------------------------------------------------------------------------------------------------- | ---- | ------------------------------------------------------------------------------------------------- |
| 4.9     | [bmcu_c_firmware_4_9.rar](/assets/files/download_center/firmware_and_source_code/bmcu_c_firmware_4_9.rar)       |      |                                                                                                   |
| 4.20    | [bmcu_c_firmware_4_20.rar](/assets/files/download_center/firmware_and_source_code/bmcu_c_firmware_4_20.zip)     |      |                                                                                                   |
| 4.23.3  | [bmcu_c_firmware_4_23_3.rar](/assets/files/download_center/firmware_and_source_code/bmcu_c_firmware_4_23_3.rar) |      |                                                                                                   |
| 4.24    |                                                                                                                 |      | [not available](/assets/files/download_center/firmware_and_source_code/abc.zip) |
| 0013    | [bmcu_c_firmware_0013.zip](/assets/files/download_center/firmware_and_source_code/bmcu_c_firmware_0013.zip)     |      | [not available](/assets/files/download_center/firmware_and_source_code/abc.zip) |
| 0013-Plus-Color-Noise-Heat-Improve    | [0013-Plus-Color-Noise-Heat-Improve.zip](/assets/files/download_center/firmware_and_source_code/0013-Plus-Color-Noise-Heat-Improve.zip)     |      | |
|0016|[BMCU-C-V0.1-0016.zip](/assets/files/download_center/firmware_and_source_code/BMCU-C-V0.1-0016.zip) |||
|0019|[BMCU-C-V0.1-0019.zip](/assets/files/download_center/firmware_and_source_code/BMCU-C-V0.1-0019.zip)|||
|0020|[BMCU-C-V0.1-0020.zip](/assets/files/download_center/firmware_and_source_code/BMCU-C-V0.1-0020.zip)|||

</details>

<details>
  <summary>Click to view firmware update log</summary>

### Update log

#### 0020

- 🛠️ Fixed incorrect LED behavior where some statuses failed to light up
- ⚙️ Resolved issue with unexpected channel online status
- 🔧 Corrected anti-disconnection mechanism (previously ineffective)
- 💡 Completely reworked the LED system:
  - Fixed flickering issues
  - Reduced LED refresh rate to improve performance
- 🔁 When a channel error is detected, the system now retries lighting up the red LED every 3 seconds.  
  This ensures that channels inserted **after** the BMCU has entered working state will still be detected visually.


#### 0014 - 0019 
- ✅ **16-color support** for P1/X1 printers (requires flashing the new firmware)
- 🛠️ Fixed the issue where **filament info could not be saved** on the latest P1 firmware (`00.01.06.62`) and slicing software (`2.1.1.52`)
- ⚙️ Refined online channel logic to prevent incorrect status detection in edge cases
- ⚡ Improved motor control: separate logic for high and low voltage scenarios

#### 0013-Plus-Color-Noise-Heat-Improve 
This version is `@XC`'s secondary development version based on 0013, optimized the following:
- Improved the problem of motor heating
- Optimized the PID parameters
- Optimized the strength of biting consumables

This version will improve the heat and noise problem effectively to some extent.

In addition, this version adds different light effects, under flashing this firmware, the motherboard will be a rainbow breathing light, and the 4020 light of the channel will change with the color of the consumables (after you change the color of the consumables through studio and handy)


#### 0013
Change Pid parametres

#### V4.23.3
Added P-Series support (still in beta)
Fixed some anomalies that caused excessive resistance in the extrusion head
Added function: press buffer and then the motor enters a short feeding mode to load consumables

#### V4.20
Fixed a possible bug with refills.

#### V4.9
BMCU-C is supported for the first time, and the secondary board uses Hall sensors to replace photoelectric sensors.
Currently there is a known bug that all channels show material, regardless of whether the subboard is connected or not

#### V3.31
The BMCU will now performs buffer jittering at the stage where it cuts off the filament

#### V3.14
From this version onwards, the BMCU can automatically detect the direction of motor rotation, eliminating the need to manually reverse the power supply depending on the model/gear being printed.

The BMCU performs a jitter test to determine the motor direction for each channel and logs it the first time the printer is connected after the firmware is flashed.

If this direction needs to be reset, it is necessary to re-flash or remove the motherboard and press reset.

#### V3.10
1. Repair motor direction judgement bug
1. Repair the bug of rewind exit component.
1. The buffer will now brake immediately when it reaches the pressure instead of stopping freely, preventing the re-feed from bursting the five passes.
1. The motor will keep moving slowly at 3mm/s within 3s after feeding to prevent the feed from not reaching the extruder head.

</details>

# 3D print files
📢 - Official version from BMCU author `@4061`
❤️ - Recommended

## BMCU-C

- ❤️ **BMCU-C improved version by @ZhuBuZaiHu (Highly recommended!!!)** - update 11th July 2025 
[Link Makerworld](https://makerworld.com/zh/models/1438783-bmcu-hall-sensor-version-370-optimized-casing#profileId-1500247)

- ❤️ **BMCU-C improved version by @Kongming**:
[Link Makerworld](https://makerworld.com/zh/models/1539594-bmcu-c-v0-2-model-kongming-optimized-final-version#profileId-1615601)

- 📢❤️ BMCU-C official model release date 11/04/2025:
[Link Makerworld](https://makerworld.com/zh/models/1322913-bmcu-c-hall-sensor-version#profileId-1359453)
[Backup link](/assets/files/print_files/BMCU_C.3mf)

- BMCU-C Higher torque version
[Link Makerworld](https://makerworld.com/zh/models/1412302-bmcu-c-hall-370-high-torque-version?from=search#profileId-1493471)

- BMCU-C Dual Micromotion Button Version By `@XC`

## BMCU-B

- 📢❤️ 370 steel ball version v3.14:
[Link Makerworld](https://makerworld.com/zh/models/1250311-bmcu-370-steel-ball-version-v3-14#profileId-1288934)
[Backup link](/assets/files/print_files/370+v2.5+original.3mf)

- 370X version by `@XC`
[Link Makerworld](https://makerworld.com/zh/models/1175070-bmcu-370x-surface-mount-micro-switch-glass-bead-tr?from=search#profileId-1184075)
> The seller on AliExpress is selling his 370X model and circuit board without informing `@XC`. If you'd like to support the developer, you can also choose to directly support his work and models.
{.is-info}


<details>
  <summary>Click here to view more</summary>
 
- 📢370 version official version V2.5:
[Link Makerworld](https://makerworld.com/zh/models/1189069-bmcu-370-version-original-v2-5#profileId-1200559)
[Backup link](/assets/files/print_files/370+v2.5+original.3mf)

- 370 extended buffer version - based on v2.5
</details>

## BMCU-A

- ❤️ QTBZ version, adjustable photoelectric block, optimised triangle clutch
[Link Makerworld](https://makerworld.com/zh/models/1147006#profileId-1150436)
[Backup link](/assets/files/print_files/BMCU%20130%20QTBZ版本.3mf)

- 130 steel ball version
[Link Makerworld](https://makerworld.com/zh/models/1109868-bmcu_130-steel-ball-and-spring-clutch-version?from=search#profileId-1106230)


<details>
  <summary>Click here to view more</summary>

### 130 version
- 📢130 Original version by the author 
[Link Makerworld](https://makerworld.com/zh/models/1147522#profileId-1151118)
[Backup link](/assets/files/print_files/130%20Original%20version%20from%20author.3mf)


- ❤️ An optimised version collected by Yuekai, almost the author's original design, with the addition of a triangle clutch using springs
[Link Makerworld](https://makerworld.com/zh/models/1162813-bmcu-130-version-an-optimized-extruder-search-comb#profileId-1291386)
[Backup link](/assets/files/print_files/BMCU%20Yuekai%20wiki.yuekai.fr.3mf)

- Brackets for A1 and A1 mini, also can be used for early version 370
[Link Makerworld](https://makerworld.com/zh/models/1147116-bracket-for-bmcu-version-130-and-version-370#profileId-1289021)
[Backup link](/assets/files/print_files/Bracket%20for%20130%20and%20early%20370.3mf)
{.grid-list}

### 180 version
- ❤️‍🔥180 version by BXT
[Link Makerworld](https://makerworld.com/zh/models/1152568-gk180v2-component-model-180bmcu-assembly#profileId-1207144)
[Backup link](/assets/files/print_files/180%20version.3mf)
{.grid-list}
  
 </details>




# F3D files

The F3D files of the original print files shared by the author are provided here, in case you wish to make additional modifications yourself to the model. Please note that some versions are missing their F3D files.


## BMCU-A
Missing

## BMCU-B

- 370 steel ball version v2.8 release date 28 Feb:
[Extruder](/assets/files/print_files/f3d/BMCU_B_extruder_v2.8_date_2_28.f3d)
{.grid-list}

## BMCU-C

- BMCU-C release date 11 Apr:
[Extruder](/assets/files/print_files/f3d/BMCU_C_extruder_date_4_11.f3d)
[Extruder with base](/assets/files/print_files/f3d/BMCU_C_full_date_4_11.f3d)
{.grid-list}

## Base

130 similar to 370

- Base v0.8 - Two-piece base adapts to BMCU-B and BMCU-C:
[Base](/assets/files/print_files/f3d/BMCU_base_v0.8.f3d)
{.grid-list}

## Bracket

todo

https://makerworld.com.cn/models/1173680


# Printer firmware backups

This section contains known working firmware versions for various Bambu Lab printers. These backups are provided for archival and reference purposes only.
At present, there is no practical need to download or use them, but they are stored here in case Bambu Lab imposes stricter limitations in the future that could restrict third-party tools or modifications.

- [P-series](/assets/files/download_center/printer_firmware_backup/p1-01.07.zip)
- [A1](/assets/files/download_center/printer_firmware_backup/a1-01.04.zip)
- [A1 mini](/assets/files/download_center/printer_firmware_backup/a1mini-01.04.zip)