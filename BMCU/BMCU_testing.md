---
title: BMCU Testing
description: 
published: true
date: 2025-02-26T10:42:16.370Z
tags: 
editor: markdown
dateCreated: 2025-02-25T12:11:39.883Z
---

> <span style="color:red; font-size:30px;"><b>⚠️WARNING</b></span>
> If you build your own PCB, please make sure that there are no short circuits, otherwise you may damage your computer/printer.
>
> Do not hot-plug or unplug the connection cable between the BMCU and the printer while the printer is powered on.
{.is-warning}


# PCB
If you build your own PCB, test it before connect to your computer or printer.

## Reference voltage value of the motherboard to ground
[pcb_voltage_to_ground](/BMCU/pcb_voltage_to_ground)


# After making PCB & Before assembling
## PCB lighting testing

Possible indicator colors of BMCU ：
<span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span> <span style="background-color:#ffdddd; color:#b30000; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">RED</span> <span style="background-color:#dfffe0; color:#006400; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">GREEN</span> <span style="background-color:#f0e0ff; color:#660099; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">PURPLE</span> <span style="background-color:#f5f5f5; color:#333333; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px; border: 1px solid #ddd;">WHITE</span>

### Mainboard Indicators

**When powered by TTL/USB ：** 
<span style="background-color:#ffdddd; color:#b30000; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">RED</span> Light ✅ : You should see Red Light to indicate the BMCU is not connected to the printer.

**When connected to the printer：** **Do not hot-plug or unplug while printer power on**
<span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span> Light ✅: Successfully receiving data from the printer, connection is normal. 
You should also see AMS system is successful regonized by the printer in the filament menu.


<span style="background-color:#ffdddd; color:#b30000; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">RED</span> Light ❌: ERROR - Not connected to the printer or communication failure with the printer.



### Sub-board Indicators
- <span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span> Light: Standby mode.
- <span style="background-color:#dfffe0; color:#006400; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">GREEN</span> Light: Waiting for material feed / Material feeding in progress.
- <span style="background-color:#f0e0ff; color:#660099; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">PURPLE</span> Light: Material is being ejected.
- <span style="background-color:#f5f5f5; color:#333333; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px; border: 1px solid #ddd;">WHITE</span> Light: Material feed successful.

### Sub-board functioning test

**When powered via TTL/USB, after connecting the sub-board to the mainboard:**
1. The RGB indicator should be <span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span> (Port 1: <span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span>, Ports 2-4: off; blinking is normal).
1. The two photoelectric sensor indicators should remain off.
1. When an object blocks the photoelectric sensor, the corresponding backside indicator should light up as <span style="background-color:#ffdddd; color:#b30000; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">RED</span>.

**When powered via the printer**
1. Both the mainboard and sub-board RGB indicators should be <span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span>.
1. The two photoelectric sensor indicators should remain off.
1. When an object blocks the photoelectric sensor, the corresponding backside indicator should light up as <span style="background-color:#ffdddd; color:#b30000; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">RED</span>.
1. The RGB indicator should remain <span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span>.

### BMCU Normal Material Feeding Light Sequence
1. <span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span> light stays on (standby).
1. <span style="background-color:#dfffe0; color:#006400; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">GREEN</span> light turns on when feeding starts, indicating the motor is working and material is entering.
1. <span style="background-color:#f5f5f5; color:#333333; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px; border: 1px solid #ddd;">WHITE</span> light turns on when material reaches the press machine, signaling the start of the old material cleaning process.
1. <span style="background-color:#f5f5f5; color:#333333; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px; border: 1px solid #ddd;">WHITE</span> light remains on, indicating successful material feeding.

### BMCU Normal Material Ejection Light Sequence
1. <span style="background-color:#f5f5f5; color:#333333; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px; border: 1px solid #ddd;">WHITE</span> light stays on (standby).
1. Machine cuts off waste material, and the press machine retracts the waste.
1. <span style="background-color:#f0e0ff; color:#660099; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">PURPLE</span> light turns on, indicating the feeding unit is retracting the waste material.
1. <span style="background-color:#d8e9ff; color:#0047b3; padding:4px 10px; border-radius:5px; font-weight:bold; font-size:18px;">BLUE</span> light remains on, signifying successful material ejection.