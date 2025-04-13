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



# PCB - Mainboard

## Mainboard original version
Most BMCU currently use this PCB.

<details>

<summary>Click here to expend</summary>

| No.    | Name                  | Package/Model              | Quantity |
| ------ | --------------------- | -------------------------- | -------- |
| PCB-1  | PH2.0 Connector       | PH2.0/10P (Horizontal SMT) | 8        |
| PCB-2  | 10kΩ Resistor Array   | 0603×4                     | 3        |
| PCB-3  | 100nF (50V) Capacitor | C0603                      | 28       |
| PCB-4  | 0.68Ω Resistor        | R1210                      | 4        |
| PCB-5  | AT8236                | SOP8                       | 4        |
| PCB-6  | Tact Switch           | KEY-SMD_B3U-1000PM         | 2        |
| PCB-7  | CH32V203C8T6 MCU      | LQFP48                     | 1        |
| PCB-8  | MX3.0 Connector       | 4pin                       | 1        |
| PCB-9  | 2.54mm Pin Header     | 4pin                       | 2        |
| PCB-10 | SMBJ24CA              | DO-214AA                   | 1        |
| PCB-11 | TP75176E-SR           | SOP8                       | 1        |
| PCB-12 | WS2812B LED           | 5050                       | 5        |
| PCB-13 | 10Ω Resistor          | 0603                       | 2        |
| PCB-14 | 120Ω Resistor         | 0603                       | 1        |
| PCB-15 | PSM712                | SOT23-3                    | 1        |
| PCB-16 | PH2.0 Cable           | 10Pin                      | 4        |
| PCB-17 | 470Ω Resistor         | 0603                       | 8        |
| PCB-18 | ITR9606 Opto Switch   | DIP                        | 8        |
| PCB-19 | AS5600 (with magnet)  | SOP8                       | 4        |
| PCB-20 | LM393                 | SOP8                       | 4        |
| PCB-21 | 1kΩ Resistor          | 0603                       | 8        |
| PCB-22 | LED                   | 0603                       | 8        |
| PCB-23 | Main Board JLC        |                            | 1        |
| PCB-24 | Sub Board JLC         |                            | 4        |


#### Power supply - choose one of them
##### If use 3.3v power module:

| No.    | Name              | Package/Model | Quantity |
| ------ | ----------------- | ------------- | -------- |
| PCB-25 | 3.3V Power Module | 24V-3.3V      | 1        |

##### If use IC:

| No.    | Name           | Package/Model | Quantity |
| ------ | -------------- | ------------- | -------- |
| PCB-26 | TPS54202DDCR   | SOT23-6       | 1        |
| PCB-27 | 47pF Capacitor | C0603         | 1        |
| PCB-28 | 15kΩ Resistor  | R0603         | 1        |
| PCB-29 | 68kΩ Resistor  | R0603         | 1        |
| PCB-30 | 22uF Capacitor | C0805         | 3        |
| PCB-31 | 10uH Inductor  | 7.3×6.8mm     | 1        |

</details>

#### If you want to try the typec version you need to:
  - 1 additional 16p typec vertical components
  - 1 additional CH340X chip 

### Mainboard with Enhanced Security Patch

# PCB - Sub-board

## Original version Sub-board

## Hall version Sub-board for BMCU-C

# Mecanical parts

## BMCU-A - 130 version:
[Mechanical Components BOM sheet download](/assets/files/bom_sheet/mechanical_components_bom.xlsx)


<details>

<summary>Click here to expend</summary>

Initial version of the BOM Sheet:

| No.    | Name                                 | Quantity | Note                                 |
| ------ | ------------------------------------ | -------- | ------------------------------------ |
| MEC-1  | MR85ZZ Bearing                       | 8        |                                      |
| MEC-2  | BMG Gear Set                         | 4        |                                      |
| MEC-3  | D5x22mm Shaft                        | 4        |                                      |
| MEC-4  | D2x10mm Shaft                        | 16       | Better have >20                      |
| MEC-5  | D2x20mm Shaft                        | 12       | Better have >20                      |
| MEC-6  | 20082B Dual Spur Gear                | 8        |                                      |
| MEC-7  | 182A Gear                            | 8        |                                      |
| MEC-8  | 242A Gear                            | 4        |                                      |
| MEC-9  | 682A Worm Gear                       | 4        |                                      |
| MEC-10 | FF-130 SH Motor                      | 4        | DC12V-4350RPM                        |
| MEC-11 | Wire (5cm or longer)                 | 8        |                                      |
| MEC-12 | 62B Bushing                          | 28       | Better have >35                      |
| MEC-13 | PC4 Pneumatic Head 6mm               | 4        |                                      |
| MEC-14 | Spring 0.5*6x10mm                    | 4        | Bigger spring for the buffer         |
| MEC-15 | Spring 0.6*4x10mm                    | 4        | Smaller spring for lever             |
| MEC-16 | M2*8 Countersunk Self-tapping Screw  | 50       |                                      |
| MEC-17 | 1.75mm Transparent Filament          | 20cm     | For guiding the light from sub-board |
| MEC-18 | M2\*4 or M2\*6 Head Screw            | 8        | For fixing the sub-board             |
| MEC-19 | M3*14 Countersunk Self-tapping Screw | 9        | Base and cable cover                 |
| MEC-20 | MX3.0-4P Mirrored Cable              | 1        |                                      |
| MEC-21 | M3*10 Standard Screw                 | 2        | For bracket                          |
| MEC-22 | M3 Nut                               | 2        | For bracket                          |

Currently we prefer to use clutches with springs, for which you will additionally require:
| No.      | Name               | Quantity | Note        |
| -------- | ------------------ | -------- | ----------- |
| 🟢➕MEC-23 | Spring 0.2\*3.5\*5 | 4        | For clutchs |

The 130 steel ball version is not an official version from the author, but in short, if you want to build the steel ball version, you will need additional:
| No.      | Name             | Quantity | Note            |
| -------- | ---------------- | -------- | --------------- |
| 🟢➕MEC-7  | 4 more 182A Gear | 4        | total 4+8=12    |
| 🟢➕MEC-24 | Spring 0.3\*4\*5 | 4        | For steel balls |
| 🟢➕MEC-25 | 5mm steel balls  | 4        |                 |

</details>

## BMCU-B - 370 motor + Photoelectric sensor

### BOM for BMCU-B v2.5 370 motors without steel ball
<details>

<summary>BOM for BMCU-B v2.5 370 motors without steel ball</summary>

| No.    | Name                                | Quantity | Note                                                |
| ------ | ----------------------------------- | -------- | --------------------------------------------------- |
| MEC-1  | MR85ZZ Bearing                      | 8        |                                                     |
| MEC-2  | BMG Gear Set                        | 4        |                                                     |
| MEC-3  | D5x22mm Shaft                       | 4        |                                                     |
| MEC-4  | D2x10mm Shaft                       | 8        | Better have >20                                     |
| MEC-5  | D2x20mm Shaft                       | 8        | Better have >20                                     |
| MEC-6  | 182A Gear                           | 8        | Better have >12                                     |
| MEC-7  | 682A Worm Gear                      | 4        |                                                     |
| MEC-8  | 370 Motor                           | 4        | DC24V-6000RPM                                       |
| MEC-9  | Wire (5cm or longer)                | 8        |                                                     |
| MEC-10 | 62B Bushing                         | 24       | Better have >35                                     |
| MEC-11 | PC4 Pneumatic Head 6mm              | 4        |                                                     |
| MEC-12 | Spring 0.6\*4\*15                   | 4        | For lever                                           |
| MEC-13 | Spring 0.6\*12\*30                  | 4        | For buffer, 0.6\*12\*30 is also recommended         |
| MEC-14 | M2*8 Countersunk Self-tapping Screw | 36       | Better have >50                                     |
| MEC-15 | 1.75mm Transparent Filament         | 20cm     |                                                     |
| MEC-16 | M2*4 or M2*6 Self-tapping Screw     | 8        | For fixing sub-boards                               |
| MEC-17 | M3*14 or M3*16 Self-tapping Screw   | 6        | 4 for fixing the extruder to the base,2 for bracket |
| MEC-18 | MX3.0-4P Mirrored Cable             | 1        |                                                     |

</details>


### BOM for BMCU-B v3.14 370 motors + steel ball

<details>

<summary>BOM for BMCU-B version v3.14 - 370 motor + steel ball</summary>

| No.    | Name                                | Quantity | Note                                        |
| ------ | ----------------------------------- | -------- | ------------------------------------------- |
| MEC-1  | MR85ZZ Bearing                      | 8        |                                             |
| MEC-2  | BMG Gear Set                        | 4        |                                             |
| MEC-3  | D5x22mm Shaft                       | 4        |                                             |
| MEC-4  | D2x10mm Shaft                       | 8        | Better have >20                             |
| MEC-5  | 🟢➕D2x20mm Shaft                     | 12       | Better have >20                             |
| MEC-7  | 🟢➕182A Gear                         | 12       | Updated to 12                               |
| MEC-9  | 682A Worm Gear                      | 4        |                                             |
| MEC-10 | 370 Motor                           | 4        | DC24V-6000RPM                               |
| MEC-11 | Wire (5cm or longer)                | 8        |                                             |
| MEC-12 | 🟢➕62B Bushing                       | 30       | Better have >35                             |
| MEC-13 | PC4 Pneumatic Head 6mm              | 4        |                                             |
| MEC-14 | 🟡✏️Spring 0.6\*4\*10                 | 4        | For lever, now spring is longer 10          |
| MEC-15 | Spring 0.6\*10\*30                  | 4        | For buffer, 0.6\*12\*30 is also recommended |
| MEC-17 | M2*8 Countersunk Self-tapping Screw | 36       | Better have >50                             |
| MEC-18 | 1.75mm Transparent Filament         | 20cm     |                                             |
| MEC-19 | M2\*4 or M2\*6 Self-tapping Screw   | 8        | For fixing sub-boards                       |
| MEC-20 | 🟡✏️M3\*14 Self-tapping Screw           | 2        | 2 for the bracket                           |
| MEC-21 | 🟢➕M3\*14 Machine screws               | 4        | For fixing the extruder to the base         |
| MEC-22 | 🟢➕M3 nuts                             | 4        | For locking extruder with machine screws    |
| MEC-23 | MX3.0-4P Mirrored Cable             | 1        |                                             |
| MEC-24 | 🟢➕5mm steel balls                     | 4        |                                             |
| MEC-25 | 🟢➕Spring 0.3\*4\*5                    | 4        | For steel balls                             |

</details>

## BMCU-C - 370 motor + Hall sensor







