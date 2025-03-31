---
title: BMCU Download Center
description: 
published: true
date: 2025-03-21T15:55:11.641Z
tags: 
editor: markdown
dateCreated: 2025-01-28T14:08:05.158Z
---

# BMCU Resources & Download center


## PCB files

### Mainboard
|    | **Classic Version**      | **Type C Version**    |
|-----------|---------|---------------------|
| PCB manufacturing files| [main board v0.4.zip](/assets/files/download_center/main_board_v0.4.zip) | [main_board_type_c_version.zip](/assets/files/download_center/main_board_type_c_version.zip)   
|Soldering aids |[Soldering_aids.zip](/assets/files/download_center/3._welding_aids.zip) | |

### Extruder (sub-board)
[extruder_(sub-board)v2.2.zip](/assets/files/download_center/extruder_(sub-board)v2.2.zip)

### Firmwares
| Version   | Firmware      |Note|Src|
|-----------|---------|-----|---|
|V0.2|[firmwarev0.2.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_v0.2.zip)  | Recommended for 130 version|
|1.21.2|[bmcu_firmware_1_21_2.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_1_21_2.zip)||
|1.26|[bmcu_firmware_1_26.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_1_26.zip)||
|2.06|[bmcu_firmware_2_06.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_2_06.zip)|For 370|
Firmware from this version onwards is adapted to the 370 version, as well as all starting to support the P-Series recognising the BMCU as an AMS system. 
| Version   | Firmware      |Note|Src|
|-----------|---------|-----|---|
|2.22|[bmcu_firmware_2_22.zip](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_2_22.zip)| |
|~~3.10~~| [~~bmcu_firmware_3-10.rar~~](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3-10.rar)|Deprecated|[src-bmcu-3-10.zip](/assets/files/download_center/firmware_and_source_code/src-bmcu-3-10.zip)|
|~~3.12~~|[~~bmcu_firmware_3_12.rar~~](/assets/files/download_center/firmware_and_source_code/bmcu_firmware_3_12.rar)|Deprecated||
|3.14|[bmcu_firmware_3_14.zip](/assets/files/download_center/firmware_and_source_code/bmcu_downloads/bmcu_firmware_3_14.zip)|Good feedback, recommended for 370|[src-bmcu-3-14.zip](/assets/files/download_center/firmware_and_source_code/bmcu_downloads/src-bmcu-3-14.zip)|
|3.31|[bmcu_firmware_3_31.rar](/assets/files/download_center/firmware_and_source_code/bmcu_downloads/bmcu_firmware_3_31.rar)|Note from author : Please be careful with five-way being jacked out, I haven't had time to test it yet||

### Changelog

#### V3.31
Now the BMCU will do a buffer jitter mode during the filament cut stage.

#### V3.14
From this version onwards there is no need to consider if we need to reverse the power supply of the motor (In iterations 130 to 370 we occasionally used a different number of gears causing occasionally we needed to reverse the power supply)
The BMCU will perform a motor jitter to determine the rotation direction of motor when the firmware is first flashed and the first connection is made to the printer

#### V3.10
1. Repair motor direction judgement bug
1. Repair the bug of rewind exit component.
1. The buffer will now brake immediately when it reaches the pressure instead of stopping freely, preventing the re-feed from bursting the five passes.
1. The motor will keep moving slowly at 3mm/s within 3s after feeding to prevent the feed from not reaching the extruder head.


## Main structure 3D print files

### 130 version
- STL files provided by the author 
[https://makerworld.com/zh/models/1147522#profileId-1151118](https://makerworld.com/zh/models/1147522#profileId-1151118)

- Latest improved 130 version 
[https://makerworld.com/zh/models/1147006#profileId-1150436](https://makerworld.com/zh/models/1147006#profileId-1150436)

- Brackets for A1 and A1 mini
[https://makerworld.com/zh/models/1147116#profileId-1150582](https://makerworld.com/zh/models/1147116#profileId-1150582)
{.grid-list}


### 370 version

- 370 version v0.1：
[https://makerworld.com/zh/models/1147008#profileId-1150439](https://makerworld.com/zh/models/1147008#profileId-1150439)
{.grid-list}

- 370 version official version V1:
https://makerworld.com/zh/models/1189069-bmcu-370-version-original-v2-5#profileId-1200559

- Brackets for A1 / A1 mini (included in this model):
https://makerworld.com/zh/models/1189069-bmcu-370-version-original-v2-5#profileId-1200559

### 




