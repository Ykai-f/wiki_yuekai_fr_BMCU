---
title: BMCU bill of materials
description: 
published: true
date: 2025-03-19T16:23:25.544Z
tags: 
editor: markdown
dateCreated: 2025-02-25T09:58:01.713Z
---

> *Note：You will always need FOUR `6x2.5mm` radial magnets, they are in fact included with the AS5600 chips in the BOM sheet of the PCB, so the author didn't list them in the mechanical sheet.
> Some of the finished PCBs do not come with this magnet. They are VERY important and BMCU can't work without them. You must purchase `RADIAL MAGNETS`.
>  ![magnet-axe.png](/assets/images/bom_sheet/magnet-axe.png =x100)  NO!!!       ![magnet-rad.png](/assets/images/bom_sheet/magnet-rad.png =x100)  YES!!!  
{.is-warning}

# BOM for PCB
Currently, all BMCUs use the same PCB regardless of motor version.
[PCB BOM sheet download](/assets/files/bom_sheet/pcb_bom.xlsx)

#### If you want to try the typec version you need to:
  - 4 additional 16p typec vertical components
  - Purchase the CH340X chip instead of the CH320V.
  - Print the base designed for the C-port

# BOM for mecanical parts
130 version :
[Mechanical Components BOM sheet download](/assets/files/bom_sheet/mechanical_components_bom.xlsx)

370 version :
to do. for now see below

#### If you want to try the 370 version you need:
- 4 x `370 motors` (6000 rpm at 24v) instad of original ff130 motor
- 4 x `0.6x4x15` springs
- 4 x `0.6x10x30` springs （Some developers have increased the length of the buffering to minimise five-way jacking out, so you can also try buy longer springs for example `0.6x10x35` or `0.6x10x50`）
- M3x16 or M3x18 self-tapping screws
- 242A gears no longer required
- (Optional) Metal gears : 8 x 0.5-mod 18-tooth metal gears, and 4 x 0.5-mod 8-tooth metal worm gears



# Notes
1. You will need 4 sections of ptfe tube for connecting BMCU and the printer extruder. Recommended length is 60cm/each , at least 50cm are needed.

1. You will need some transparent, colorless filaments for light guiding, only 4 of approx. 10 cm are needed so maybe no need to buy a whole row.




