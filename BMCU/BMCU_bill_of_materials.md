---
title: BMCU bill of materials
description: 
published: true
date: 2025-04-01T18:25:14.105Z
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


<details>

<summary>BOM for BMCU's PCB</summary>

| No.    | Name                    | Package/Model              | Quantity |
|--------|-------------------------|----------------------------|----------|
| PCB-1  | PH2.0 Connector         | PH2.0/10P (Horizontal SMT) | 8        |
| PCB-2  | 10kΩ Resistor Array     | 0603×4                     | 3        |
| PCB-3  | 100nF (50V) Capacitor   | C0603                      | 28       |
| PCB-4  | 0.68Ω Resistor          | R1210                      | 4        |
| PCB-5  | AT8236                  | SOP8                       | 4        |
| PCB-6  | Tact Switch             | KEY-SMD_B3U-1000PM         | 2        |
| PCB-7  | CH32V203C8T6 MCU        | LQFP48                     | 1        |
| PCB-8  | MX3.0 Connector         | 4pin                       | 1        |
| PCB-9  | 2.54mm Pin Header       | 4pin                       | 2        |
| PCB-10 | SMBJ24CA                | DO-214AA                   | 1        |
| PCB-11 | TP75176E-SR             | SOP8                       | 1        |
| PCB-12 | WS2812B LED             | 5050                       | 5        |
| PCB-13 | 10Ω Resistor            | 0603                       | 2        |
| PCB-14 | 120Ω Resistor           | 0603                       | 1        |
| PCB-15 | PSM712                  | SOT23-3                    | 1        |
| PCB-16 | PH2.0 Cable             | 10Pin                      | 4        |
| PCB-17 | 470Ω Resistor           | 0603                       | 8        |
| PCB-18 | ITR9606 Opto Switch     | DIP                        | 8        |
| PCB-19 | AS5600 (with magnet)    | SOP8                       | 4        |
| PCB-20 | LM393                   | SOP8                       | 4        |
| PCB-21 | 1kΩ Resistor            | 0603                       | 8        |
| PCB-22 | LED                     | 0603                       | 8        |
| PCB-23 | Main Board JLC          |                            | 1        |
| PCB-24 | Sub Board JLC           |                            | 4        |


#### Power supply - choose one of them
##### If use 3.3v power module:

| No.    | Name                         | Package/Model              | Quantity | 
|--------|------------------------------|----------------------------|----------|
| PCB-25 | 3.3V Power Module            | 24V-3.3V                   | 1        |

##### If use IC:

| No.    | Name                         | Package/Model              | Quantity | Recommended Qty  |
|--------|-------------|-------------|----------|------------------|
| PCB-26 | TPS54202DDCR | SOT23-6     | 1        | -                |
| PCB-27 | 47pF Capacitor | C0603     | 1        | -                |
| PCB-28 | 15kΩ Resistor | R0603     | 1        | -                |
| PCB-29 | 68kΩ Resistor | R0603     | 1        | -                |
| PCB-30 | 22uF Capacitor | C0805    | 3        | -                |
| PCB-31 | 10uH Inductor | 7.3×6.8mm | 1        | -                |

</details>

#### If you want to try the typec version you need to:
  - 1 additional 16p typec vertical components
  - 1 additional CH340X chip 



# BOM for mecanical parts
130 version :
[Mechanical Components BOM sheet download](/assets/files/bom_sheet/mechanical_components_bom.xlsx)

370 version :
to do. for now see below

#### If you want to try the 370 version you need:
- 4 x `370 motors` (6000 rpm at 24v) instad of original ff130 motor
- 4 x `0.6x4x10` springs
- 4 x `0.6x10x30` springs （Some developers have increased the length of the buffering to minimise five-way jacking out, so you can also try buy longer springs for example `0.6x10x35` or `0.6x10x50`）
- M3x16 or M3x18 self-tapping screws
- 242A gears no longer required
- (Optional) Metal gears : 8 x 0.5-mod 18-tooth metal gears, and 4 x 0.5-mod 8-tooth metal worm gears

For 370 steel ball version you will still need :
- 0.3×4×5 springs for steel balls x4
- 5mm steel ball x4
- 12 x 182A gears
- m3 nuts x2
- m3 machine thread screws x4




# Notes
1. You will need 4 sections of ptfe tube for connecting BMCU and the printer extruder. Recommended length is 60cm/each , at least 50cm are needed.

1. You will need some transparent, colorless filaments for light guiding, only 4 of approx. 10 cm are needed so maybe no need to buy a whole row.




