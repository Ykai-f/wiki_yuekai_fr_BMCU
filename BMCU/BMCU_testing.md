---
title: BMCU Testing
description: 
published: true
date: 2025-04-14T12:03:39.385Z
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

Otherwise you might see...

![pcb_voltage_to_ground](/assets/images/gif/1.gif)


## Reference voltage value of the motherboard to ground
[pcb_voltage_to_ground](/BMCU/pcb_voltage_to_ground)

# PCB lighting testing

Possible indicator colors of BMCU ：
<span class="indicator indicator-blue">BLUE</span>  <span class="indicator indicator-red">RED</span>  <span class="indicator indicator-green">GREEN</span>  <span class="indicator indicator-purple">PURPLE</span>  <span class="indicator indicator-white">WHITE</span>

### Mainboard Indicators

**When powered by TTL/USB ：** 
<span class="indicator indicator-red">RED</span> Light ✅ : You should see Red Light to indicate the BMCU is not connected to the printer.

**When connected to the printer：** **Do not hot-plug or unplug while printer power on**
<span class="indicator indicator-blue">BLUE</span> Light ✅: Successfully receiving data from the printer, connection is normal. 
You should also see AMS system is successful regonized by the printer in the filament menu.


<span class="indicator indicator-red">RED</span> Light ❌: ERROR - Not connected to the printer or communication failure with the printer.



### Sub-board Indicators
- <span class="indicator indicator-blue">BLUE</span> Light: Standby mode.
- <span class="indicator indicator-green">GREEN</span> Light: Waiting for material feed / Material feeding in progress.
- <span class="indicator indicator-purple">PURPLE</span> Light: Material is being ejected.
- <span class="indicator indicator-white">WHITE</span> Light: Material feed successful.

### Sub-board functioning test

**When powered via TTL/USB, after connecting the sub-board to the mainboard:**
 
- **If you are running BMCU-A's firmware** : The RGB indicator should be <span class="indicator indicator-blue">BLUE</span>, Ports 2-4: off; blinking is normal).
- **If you are running BMCU-B or BMCU-C's firmware** : All the RGB indicators should be <span class="indicator indicator-red">RED</span>.

- The two photoelectric sensor indicators should remain off.
- When an object blocks the photoelectric sensor, the corresponding backside indicator should light up as <span class="indicator indicator-red">RED</span>.

> Since version 3.14, when the BMCU is powered on standby, there are two possible se for the indicator light on the sub board: 
> <span class="indicator indicator-blue">BLUE</span> -> ok
> 
> <span class="indicator indicator-red">RED</span> -> magnet sensing failure, check if the radial magnet is too far away from sub-board, or the as5600 chip not working nomolly.

**When powered via the printer**
1. Both the mainboard and sub-board RGB indicators should be <span class="indicator indicator-blue">BLUE</span>.
1. The two photoelectric sensor indicators should remain off.
1. When an object blocks the photoelectric sensor, the corresponding backside indicator should light up as <span class="indicator indicator-red">RED</span>.
1. The RGB indicator should remain <span class="indicator indicator-blue">BLUE</span>.


### BMCU Normal Material Feeding Light Sequence
1. <span class="indicator indicator-blue">BLUE</span> light stays on (standby).
1. <span class="indicator indicator-green">GREEN</span> light turns on when feeding starts, indicating the motor is working and material is entering.
1. <span class="indicator indicator-white">WHITE</span> light turns on when material reaches the press machine, signaling the start of the old material cleaning process.
1. <span class="indicator indicator-white">WHITE</span> light remains on, indicating successful material feeding.

### BMCU Normal Material Ejection Light Sequence
1. <span class="indicator indicator-white">WHITE</span> light stays on (standby).
1. Machine cuts off waste material, and the press machine retracts the waste.
1. <span class="indicator indicator-purple">PURPLE</span> light turns on, indicating the feeding unit is retracting the waste material.
1. <span class="indicator indicator-blue">BLUE</span> light remains on, signifying successful material ejection.