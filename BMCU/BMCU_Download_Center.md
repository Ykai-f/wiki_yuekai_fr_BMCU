---
title: BMCU Download Center
description: 
published: true
date: 2025-05-13T00:11:36.881Z
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

> Some users have reported that **new versions of the mainboard** may have issues, such as unexpected reboots or certain channels malfunctioning despite proper soldering.
>
>The developer is currently working on software-level fixes to address these problems.
>
>If you’d like to try the Hall sensor version, for now you can also try to use the **original version of the mainboard**  with the **Hall sensor sub-board**.
{.is-warning}


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
- **BMCU-C** : Test 0013 [bmcu_c_firmware_0013.zip](/assets/files/download_center/firmware_and_source_code/bmcu_c_firmware_0013.zip)

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
| 4.24    |                                                                                                                 |      | [src-bmcu-c-4.24.zip](/assets/files/download_center/firmware_and_source_code/src-bmcu-c-4.24.zip) |
| 0013    | [bmcu_c_firmware_0013.zip](/assets/files/download_center/firmware_and_source_code/bmcu_c_firmware_0013.zip)     |      | [src-BMCU-C-0013.zip](/assets/files/download_center/firmware_and_source_code/src-BMCU-C-0013.zip) |

</details>

<details>
  <summary>Click to view firmware update log</summary>

### Update log

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

## BMCU-A

### 130 version
- 130 Original version by the author 
[Link Makerworld](https://makerworld.com/zh/models/1147522#profileId-1151118)
[Backup link](/assets/files/print_files/130%20Original%20version%20from%20author.3mf)

- ❤️‍🔥QTBZ version, adjustable photoelectric block, optimised triangle clutch
[Link Makerworld](https://makerworld.com/zh/models/1147006#profileId-1150436)
[Backup link](/assets/files/print_files/BMCU%20130%20QTBZ版本.3mf)

- ❤️‍🔥An optimised version collected by Yuekai, almost the author's original design, with the addition of a triangle clutch using springs
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

## BMCU-B
- 370 version official version V2.5:
[Link Makerworld](https://makerworld.com/zh/models/1189069-bmcu-370-version-original-v2-5#profileId-1200559)
[Backup link](/assets/files/print_files/370+v2.5+original.3mf)

- ❤️‍🔥370 steel ball version v3.14:
[Link Makerworld](https://makerworld.com/zh/models/1250311-bmcu-370-steel-ball-version-v3-14#profileId-1288934)
[Backup link](/assets/files/print_files/370+v2.5+original.3mf)

- Brackets for A1 / A1 mini (included in this model):
[Link Makerworld](https://makerworld.com/zh/models/1147116-bracket-for-bmcu-version-130-and-version-370#profileId-1289021)
[Backup link](/assets/files/print_files/370+steel+ball+version+3.14.3mf)
{.grid-list}

## BMCU-C

- BMCU-C model release date 11/04/2025:
[Link Makerworld](https://makerworld.com/zh/models/1322913-bmcu-c-hall-sensor-version#profileId-1359453)
[Backup link](/assets/files/print_files/BMCU_C.3mf)
{.grid-list}


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

- Base v0.8 - Two-piece base adapts to BMCU-B and BMCU-C:
[Base](/assets/files/print_files/f3d/BMCU_base_v0.8.f3d)
{.grid-list}


# Printer firmware backups

This section contains known working firmware versions for various Bambu Lab printers. These backups are provided for archival and reference purposes only.
At present, there is no practical need to download or use them, but they are stored here in case Bambu Lab imposes stricter limitations in the future that could restrict third-party tools or modifications.

- [P-series](/assets/files/download_center/printer_firmware_backup/p1-01.07.zip)
- [A1](/assets/files/download_center/printer_firmware_backup/a1-01.04.zip)
- [A1 mini](/assets/files/download_center/printer_firmware_backup/a1mini-01.04.zip)