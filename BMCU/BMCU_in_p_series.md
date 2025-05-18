---
title: BMCU with P/X series
description: 
published: true
date: 2025-05-18T00:50:05.392Z
tags: 
editor: markdown
dateCreated: 2025-03-20T14:42:09.077Z
---

This page still in progress because I don't have all the information for BMCU on P series.
{.is-warning}


> Update 5th May
> In firmware versions :
**01.08.00.00** for the **P series**
**01.09.00.00 (20250429)** for the **X series**
>
>Bambulab has added support for the updated AMS model like AMS 2, which involved changes to the communication protocol between the AMS system and the printer. 
>
>As a result, BMCU currently does not function properly (e.g., unable to modify filament settings). It is unclear how soon BMCU's author will respond to these changes. If you intend to keep your P/X printer updated with the latest firmware, we recommend not relying on BMCU at this time.
>
>The **A-series** is not affected at the moment, according to Bambulab the adaptation programme for the newer AMS for the A-series is still a few months away.
{.is-danger}


## BMCU Version Adaptation Status

- **BMCU-A**: Not supported; no plans for future adaptation.
- **BMCU-B**: Fully supported and running well on the P-Series.
- **BMCU-C**: Testing.

## If using externe 5 way

You will need a bambu 4-in-1 ptfe adapter or anything similar.
![4-in-1 adapter](/assets/images/p_series/4_in_1_adapter.png =x300)

![bmcu_p_ext_5way.png](/assets/images/p_series/bmcu_p_ext_5way.png =x300)

And you need a firmware to make the rejection behaviour longer so that the filament can always exit to the outside of the bambu 4-in-1 ptfe adapter.

## if using internal 5 way

![internal 5 way 1](/assets/images/p_series/p1_int_5way_1.jpg =x300)
![internal 5 way 2](/assets/images/p_series/p1_int_5way_2.jpg =x300)


## Firmwares

These firmwares are modified by XC `@星尘`

### BMCU-B

#### 3.14
Externe 5 way:
- [P1S_RetModified_BMCU370-3.14_15s_Ext5Way.rar](/assets/files/download_center/p_series/P1S_RetModified_BMCU370-3.14_15s_Ext5Way.rar)
- [P1S_RetModified_BMCU370_3.14_14s_Ext5Way.rar](/assets/files/download_center/p_series/P1S_RetModified_BMCU370_3.14_14s_Ext5Way.rar)

Internal 5 way:
- [P1S_RetModified_BMCU370_3.14_4s_Int5Way.rar](/assets/files/download_center/p_series/P1S_RetModified_BMCU370_3.14_4s_Int5Way.rar)
- [P1S_RetModified_BMCU370_3.14_3.5s_Int5Way.rar](/assets/files/download_center/p_series/P1S_RetModified_BMCU370_3.14_3.5s_Int5Way.rar)

### BMCU-C

#### 4.24
Using internal 5 way:

- [P_Hall_4_24_Int5Way.bin.zip](/assets/files/download_center/p_series/P_Hall_4_24_Int5Way.bin.zip) -  **Different springs required: `WD0.6 OD12 L30 mm` for buffer and `WD0.6 OD4 L15` for lever**

## Using AMS + BMCU or more than one BMCU

### AMS + BMCU

The principle of the BMCU is to directly simulate the AMS device to communicate with the printer, it is possible to use AMS + BMCU on the P-Series, (I can't say for sure for newer devices like AMS 2)

See the official Bambulab tutorial for using two AMS https://wiki.bambulab.com/en/x1/manual/Connect-AMS-Hub-and-multi-AMS

Since the BMCU only has one 4pin connector, you need to connect the AMS directly to the AMS Hub, and then connect the BMCU to the AMS.

### 2\*BMCU

Please note that it is not possible to use two BMCUs directly on the P-Series.

Altertive : BMCU-Hub to connect 4 BMCUs-> to update
