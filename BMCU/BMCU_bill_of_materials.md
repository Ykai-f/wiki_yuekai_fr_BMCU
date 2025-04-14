---
title: BMCU bill of materials
description: 
published: true
date: 2025-04-14T09:03:53.410Z
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

![mainboard_origina_version.png](/assets/images/bmcu_branch/mainboard_origina_version.png =x300)

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
| PCB-8  | MX3.0 Connector       | 4pin  2*2                  | 1        |
| PCB-9  | 2.54mm Pin Header     | 4pin 2\*2 or 8pin 2\*4     | 2        |
| PCB-10 | SMBJ24CA              | DO-214AA                   | 1        |
| PCB-11 | TP75176E-SR           | SOP8                       | 1        |
| PCB-12 | WS2812B LED           | 5050                       | 5        |
| PCB-13 | 10Ω Resistor          | 0603                       | 2        |
| PCB-14 | 120Ω Resistor         | 0603                       | 1        |
| PCB-15 | PSM712                | SOT23-3                    | 1        |
| PCB-16 | PH2.0 Cable           | 10Pin                      | 4        |


#### Power supply - choose one of them
##### If use 3.3v power module:

| No.    | Name              | Package/Model | Quantity |
| ------ | ----------------- | ------------- | -------- |
| PCB-17 | 3.3V Power Module | 24V-3.3V      | 1        |

##### If use IC:

| No.    | Name           | Package/Model | Quantity |
| ------ | -------------- | ------------- | -------- |
| PCB-18 | TPS54202DDCR   | SOT23-6       | 1        |
| PCB-19 | 47pF Capacitor | C0603         | 1        |
| PCB-20 | 15kΩ Resistor  | R0603         | 1        |
| PCB-21 | 68kΩ Resistor  | R0603         | 1        |
| PCB-22 | 22uF Capacitor | C0805         | 3        |
| PCB-23 | 10uH Inductor  | 7.3×6.8mm     | 1        |

</details>

### Mainboard with Enhanced Security Patch

![mainboard_enhanced_security_patch.png](/assets/images/bmcu_branch/mainboard_enhanced_security_patch.png =x300)

<details>

<summary>Click here to expend</summary>

| No.    | Name            | Package/Model              | Quantity |
| ------ | --------------- | -------------------------- | -------- |
| PCB_1  | 22uF            | C1206                      | 1        |
| PCB_2  | 100nF           | C0603                      | 12       |
| PCB_3  | MX3.0 Connector | 4pin 2*2                   | 1        |
| PCB_4  | PH2.0 Connector | PH2.0/10P (Horizontal SMT) | 4        |
| PCB_5  | SMBJ24CA        | SMB_L4.6-W3.6-LS5.3-BI     | 1        |
| PCB_6  | PSM712-LF-T7    | SOT-23-3_L3.0-W1.7-P0.95   | 1        |
| PCB_7  | 1N5819WS        | SOD-323_L1.8-W1.3-LS2.5    | 1        |
| PCB_8  | SS54            | SMA_L4.4-W2.8-LS5.4        | 1        |
| PCB_9  | HDR-M_2.54_1x4P | HDR-TH_4P-P2.54-V-M        | 2        |
| PCB_10 | WS2812B         | 5050                       | 1        |
| PCB_11 | AO3401A         | SOT-23_L2.9-W1.3-P1.90     | 1        |
| PCB_12 | 680mΩ           | R1210                      | 4        |
| PCB_13 | 10Ω             | R0603                      | 3        |
| PCB_14 | 120Ω            | R0603                      | 1        |
| PCB_15 | 470Ω            | R0603                      | 1        |
| PCB_16 | 10kΩ            | RES-ARRAY-SMD_0603         | 3        |
| PCB_17 | Tact Switch     | KEY-SMD_B3U-1000PM         | 2        |
| PCB_18 | CH32V203C8T6    | LQFP-48_L7.0-W7.0          | 1        |
| PCB_19 | TP75176E-SR     | SOP-8_L4.9-W3.9            | 1        |
| PCB_20 | AT8236          | ESOP-8_L4.9-W3.9           | 4        |

#### Power supply - choose one of them
##### If use 3.3v power module(recommended):

| No.    | Name              | Package/Model | Quantity |
| ------ | ----------------- | ------------- | -------- |
| PCB-28 | 3.3V Power Module | 24V-3.3V      | 1        |

##### If use IC:
| No.    | Name         | Package/Model      | Quantity |
| ------ | ------------ | ------------------ | -------- |
| PCB_21 | 10uH         | IND-SMD_L7.3-W6.8  | 1        |
| PCB_22 | 100nF        | C0603              | 1        |
| PCB_23 | 47pF         | C0603              | 1        |
| PCB_24 | 15kΩ         | R0603              | 1        |
| PCB_25 | 68kΩ         | R0603              | 1        |
| PCB_26 | 22uF         | C0805              | 2        |
| PCB_27 | TPS54202DDCR | SOT-23-6_L2.9-W1.6 | 1        |

</details>

---

# PCB - Sub-board

> The number you see has been multiplied by four extruder channels.

## Original version Sub-board for BMCU-A and BMCU-B

![subboard_original_version_1.png](/assets/images/bmcu_branch/subboard_original_version_1.png =x200) ![subboard_original_version_2.png](/assets/images/bmcu_branch/subboard_original_version_2.png =x200) 

<details>

<summary>Click here to expend</summary>

| No.    | Name                       | Package/Model                      | Quantity |
| ------ | -------------------------- | ---------------------------------- | -------- |
| PCB_1  | 100nF                      | C0603                              | 12        |
| PCB_2  | PH2.0 Connector            | PH2.0/10P (Horizontal SMT)         | 4        |
| PCB_3  | WS2812B                    | 5050                               | 4        |
| PCB_4  | LED_0603-R                 | LED_0603                           | 8        |
| PCB_5  | 470Ω                       | R0603                              | 8        |
| PCB_6  | 1kΩ                        | R0603                              | 8        |
| PCB_7  | 10kΩ                       | RES-ARRAY-SMD_0603-8P-L3.2-W1.6-BL | 8        |
| PCB_8  | AS5600(with radial magnet) | SOIC-8_L4.9-W3.9-P1.27-LS6.0-BL    | 4        |
| PCB_9  | LM393DR2G                  | SOIC-8_L5.0-W4.0-P1.27-LS6.0-BL    | 4        |
| PCB_10 | ITR9606                    | OPTO-TH_4P_ITR9606                 | 8        |


</details>

## Hall version Sub-board for BMCU-C

![subboard_hall_sensor.png](/assets/images/bmcu_branch/subboard_hall_sensor.png =x300)

<details>

<summary>Click here to expend</summary>

| No.    | Name                       | Package/Model                     | Quantity |
| ------ | -------------------------- | --------------------------------- | -------- |
| PCB_1  | 100nF                      | C0603                             | 28        |
| PCB_2  | PH2.0 Connector            | PH2.0/10P (Horizontal SMT)        | 4        |
| PCB_3  | WS2812B                    | 5050                              | 4        |
| PCB_4  | WS2812B                    | 4020                              | 4|
| PCB_5  | 470Ω                       | R0603                             | 8        |
| PCB_6  | 10kΩ                       | R0603                             | 16        |
| PCB_7  | AS5600(with radial magnet) | SOIC-8_L4.9-W3.9-P1.27-LS6.0-BL   | 4        |
| PCB_8  | ITR9606                    | OPTO-TH_4P_ITR9606                | 4        |
| PCB_9  | OH49E-S                    | SOT-23-3_L2.9-W1.6-P1.90-LS2.8-BR | 4        |
| PCB_10 | LMV358                     | SOP-8_L4.9-W3.9-P1.27-LS6.0-BL    | 4        |


</details>

# Mecanical parts

## BMCU-A - 130 version:

<details>

<summary>Click here to expend</summary>

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
| MEC-14 | Spring 0.5*6x10mm - W0.5 OD6 L10 mm                    | 4        | Bigger spring for the buffer         |
| MEC-15 | Spring 0.6*4x10mm - W0.6 OD4 L10 mm                    | 4        | Smaller spring for lever             |
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

<summary>Click here to expend</summary>

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
| MEC-12 | Spring 0.6\*4\*15 - W0.6 OD4 L15 mm                   | 4        | For lever                                           |
| MEC-13 | Spring 0.6\*10\*30 - W0.6 OD10 L30 mm                  | 4        | For buffer, 0.6\*12\*30 is also recommended         |
| MEC-14 | M2*8 Countersunk Self-tapping Screw | 36       | Better have >50                                     |
| MEC-15 | 1.75mm Transparent Filament         | 20cm     |                                                     |
| MEC-16 | M2\*4 or M2\*6 Self-tapping Screw     | 8        | For fixing sub-boards                               |
| MEC-17 | M3\*14 or M3\*16 Self-tapping Screw   | 6        | 4 for fixing the extruder to the base,2 for bracket |
| MEC-18 | MX3.0-4P Mirrored Cable             | 1        |                                                     |

</details>


### BOM for BMCU-B v3.14 370 motors + steel ball

<details>

<summary>Click here to expend</summary>

| No.    | Name                                | Quantity | Note                                        |
| ------ | ----------------------------------- | -------- | ------------------------------------------- |
| MEC-1  | MR85ZZ Bearing                      | 8        |                                             |
| MEC-2  | BMG Gear Set                        | 4        |                                             |
| MEC-3  | D5x22mm Shaft                       | 4        |                                             |
| MEC-4  | D2x10mm Shaft                       | 8        | Better have >20                             |
| MEC-5  | D2x20mm Shaft                     | 12       | Better have >20                             |
| MEC-7  | 182A Gear                         | 12       | Updated to 12                               |
| MEC-9  | 682A Worm Gear                      | 4        |                                             |
| MEC-10 | 370 Motor                           | 4        | DC24V-6000RPM                               |
| MEC-11 | Wire (5cm or longer)                | 8        |                                             |
| MEC-12 | 62B Bushing                       | 30       | Better have >35                             |
| MEC-13 | PC4 Pneumatic Head 6mm              | 4        |                                             |
| MEC-14 | Spring 0.6\*4\*10 - W0.6 OD4 L10 mm                 | 4        | For lever, now spring is longer 10          |
| MEC-15 | Spring 0.6\*10\*30 - W0.6 OD10 L30 mm                  | 4        | For buffer, 0.6\*12\*30 is also recommended |
| MEC-17 | M2*8 Countersunk Self-tapping Screw | 36       | Better have >50                             |
| MEC-18 | 1.75mm Transparent Filament         | 20cm     |                                             |
| MEC-19 | M2\*4 or M2\*6 Self-tapping Screw   | 8        | For fixing sub-boards                       |
| MEC-20 | M3\*14 Self-tapping Screw         | 2        | 2 for the bracket                           |
| MEC-21 | M3\*14 Machine screws             | 4        | For fixing the extruder to the base         |
| MEC-22 | M3 nuts                           | 4        | For locking extruder with machine screws    |
| MEC-23 | MX3.0-4P Mirrored Cable             | 1        |                                             |
| MEC-24 | 5mm steel balls                   | 4        |                                             |
| MEC-25 | Spring 0.3\*4\*5 - W0.3 OD4 L5 mm                  | 4        | For steel balls                             |

</details>

## BMCU-C - 370 motor + Hall sensor

<details>

<summary>Click here to expend</summary>

| No.    | Name                                | Quantity | Note                                                       |
|--------|-------------------------------------|----------|------------------------------------------------------------|
| MEC_1  | MR85ZZ bearing                      | 8        |                                               |
| MEC_2  | BMG gear kit                        | 4        |                                                            |
| MEC_3  | D5x22mm shaft                       | 4        | This shaft has accuracy problems, pick a small tolerance before using it.                        |
| MEC_4  | D2x20mm shaft                       | 16       |                                                |
| MEC_5  | 182A gear                           | 12       | Better have some more for backup                                 |
| MEC_6  | 682A worm gear                      | 4        |                                                |
| MEC_7  | RS370 motor 24V 6000RPM             | 4        |                                                |
| MEC_8  | M3*5 metric screw                   | 4        | For fixing the motor                                               |
| MEC_9  | Wires                               | 8        | >=5cm                                                 |
| MEC_10 | 62B shaft sleeve                    | 32       |                                                            |
| MEC_11 | PC4 pneumatic fitting 6mm           | 4        | Or 8 if you want to install both side                               |
| MEC_12 | 5MM stainless steel balls           | 4        |                                                            |
| MEC_13 | Spring 0.3\*4\*5mm - W0.3 OD4 L5 mm   | 4        | For steel ball                                                  |
| MEC_14 | Spring 0.6\*4x10mm - W0.6 OD4 L10 mm                | 4        | For lever                                                  |
| MEC_15 | Spring 0.7\*12\*25mm - 	W0.7 OD12 L25 mm                 | 8        | For buffer，in case insufficient pressure, replace by D0.8           |
| MEC_16 | M2*8 countersunk self-tapping screw | 48       |                                                            |
| MEC_17 | 1.5mm optical fiber                 | 20cm       | or transparant PETG filament                                   |
| MEC_18 | N35 3*20mm cylindrical magnet       | 8        | You can also buy two 3*10 sucked together for future use with CMCUs |
| MEC_19 | M2*8 countersunk self-tapping screw | 4        |                                  |
| MEC_20 | M3*14 countersunk machine screw     | 4        |                                                            |
| MEC_21 | M3 hex nut                          | 4        |                                                            |
| MEC_22 | MX3.0-4P mirrored cable             | 1        |                                                            |


</details>


