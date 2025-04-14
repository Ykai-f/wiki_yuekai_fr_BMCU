---
title: BMCU Download Center
description: 
published: true
date: 2025-04-14T13:30:56.503Z
tags: 
editor: markdown
dateCreated: 2025-01-28T14:08:05.158Z
---

# PCB files

## Mainboard
| Version                                    | PCB manufacturing files                                                                                                | Soldering aids                                                                                                           |
| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| **Mainboard Original Version**             | [pcb_gerber_main_board_v0.4.zip](/assets/files/download_center/pcb_files/pcb_gerber_main_board_v0.4.zip)                                     | [soldering_aids_mainboard_v0.4.rar](/assets/files/download_center/pcb_files/soldering_aids_mainboard_v0.4.rar)                                       |
| **Mainboard with Enhanced Security Patch** | [pcb_gerber_mainboard_enhanced_security_patch.zip](/assets/files/download_center/pcb_files/pcb_gerber_mainboard_enhanced_security_patch.zip) | [soldering_aids_mainboard_enhanced_security_patch.rar](/assets/files/download_center/pcb_files/soldering_aids_mainboard_enhanced_security_patch.rar) |  |

## Extruder (sub-board)

| version                 | PCB manufacturing files                                                                          | Soldering aids                                                                                           |
| ----------------------- | ------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------- |
| **Original version**    | [pcb_gerber_sub_board_v2_2.zip](/assets/files/download_center/pcb_files/pcb_gerber_sub_board_v2_2.zip)                 | [soldering_aids_sub_board_original_version.rar](/assets/files/download_center/pcb_files/soldering_aids_sub_board_original_version.rar) |
| **Hall sensor Version** | [pcb_gerber_sub_board_hall.zip](/assets/files/download_center/pcb_files/pcb_gerber_sub_board_hall.zip) | [soldering_aids_sub_board_hall.rar](/assets/files/download_center/pcb_files/soldering_aids_sub_board_hall.rar)                         |


# Firmwares

## Firmwares for BMCU-A
| Version | Firmware                                                                                                    | Note                          | Src |
| ------- | ----------------------------------------------------------------------------------------------------------- | ----------------------------- | --- |
| V0.2    | [firmwarev0.2.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_v0.2.zip)           | ⭐⭐⭐Recommended for **BMCU-A** |
| 1.21.2  | [bmcu_firmware_1_21_2.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_1_21_2.zip) |                               |
| 1.26    | [bmcu_firmware_1_26.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_1_26.zip)     |                               |


## Firmwares for BMCU-B
Firmware from this version onwards is adapted to the BMCU-B aka 370 version aka,
also starting to support the P-Series recognising the BMCU as an AMS system. 
| Version  | Firmware                                                                                                    | Note                                                          | Src                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| 2.06     | [bmcu_firmware_2_06.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_2_06.zip)     | For 370                                                       |
| 2.22     | [bmcu_firmware_2_22.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_2_22.zip)     |                                                               |
| ~~3.10~~ | [~~bmcu_firmware_3-10.rar~~](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3-10.rar) | Deprecated                                                    | [src-bmcu-3-10.zip](/assets/files/download_center/firmware_and_source_code/src-bmcu-3-10.zip) |
| ~~3.12~~ | [~~bmcu_firmware_3_12.rar~~](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3_12.rar) | Deprecated                                                    |                                                                                               |
| 3.14     | [bmcu_firmware_3_14.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3_14.zip)     | ⭐⭐⭐Recommended for **BMCU-B** aka 370 version                 | [src-bmcu-3-14.zip](/assets/files/download_center/firmware_and_source_code/src-bmcu-3-14.zip) |
| 3.31     | [bmcu_firmware_3_31.rar](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3_31.rar)     | Note from author :possible five-way top-out problem, untested |

## Firmware for BMCU-C
Firmware from this version adapted to BMCU-C

| Version | Firmware                                                                                                    | Note          | Src |
| ------- | ----------------------------------------------------------------------------------------------------------- | ------------- | --- |
| 4.9     | [bmcu_c_firmware_4_9.rar](/assets/files/download_center/firmware_and_source_code/bmcu_c_firmware_4_9.rar)   | test firmware |     |
| 4.13    | [bmcu_c_firmware_4_13.rar](/assets/files/download_center/firmware_and_source_code/bmcu_c_firmware_4_13.rar) | test firmware |     |

### Changelog

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

- 370 version official v2.5 extented buffer version (require some longer springs 0.6\*10\*50 or longer)
Link Makerworld not yet, if you printed this please send me some photos :p
[Backup link](/assets/files/print_files/370%20v2.5%20extended%20version.3mf)

- ❤️‍🔥370 steel ball version v3.14:
[Link Makerworld](https://makerworld.com/zh/models/1250311-bmcu-370-steel-ball-version-v3-14#profileId-1288934)
[Backup link](/assets/files/print_files/370+v2.5+original.3mf)

- Brackets for A1 / A1 mini (included in this model):
[Link Makerworld](https://makerworld.com/zh/models/1147116-bracket-for-bmcu-version-130-and-version-370#profileId-1289021)
[Backup link](/assets/files/print_files/370+steel+ball+version+3.14.3mf)
{.grid-list}

## BMCU-C





