---
title: Just got a BMCU / How to start using BMCU
description: 
published: true
date: 2025-04-23T15:20:52.617Z
tags: 
editor: markdown
dateCreated: 2025-03-31T11:20:11.177Z
---

todo

> <span style="color:red; font-size:30px;"><b>⚠️WARNING</b></span>
> Do not hot-plug or unplug the connection cable between the BMCU and the printer while the printer is powered on.
{.is-warning}

### First use

1. Connect the BMCU to the AMS connector on the back of the printer with the **printer off**, for A1 you can choose either connector (they are the same)
2. You should see all the lights on the main board of the BMCU and the extruder turn **blue**, and the presence of the AMS system should be displayed in the filament menu, or if there are no filament inserted, it should show that there are no consumables present for any channel.
3. Press the lever on the BMCU channel and insert the filament until it passes through the other end. Unlike with an external spool, you should not insert the filament to reach inside the AMS Lite Hub, which will result in an error.
    If you notice that the supplies are having trouble reaching the other end, which is common, here are a few tips:
    1. Sharpen the top of the filament
    2. Press the buffer or pull the buffer out and continue to try to insert the filament
    3. Try removing the PTFE tube and reinstalling it after the filament comes out

### Known defects
- some channels will always show the presence of filament, for more information check this section : 

### If you are using BMCU-B and you found your 5way(AMS Lite Hub) pops up 
Like this:
![5_way_pop_up.gif](/assets/images/gif/5way_pop_up.gif =x300)

One of the solutions is as follows.
This option is recommended but not always required. If you are not experiencing problems with five-way it is usually not necessary to do this additionally.

This option is a separate setting for filaments, which means you will need to set it for all your filaments multiple times.

![deactive_retraction_when_cut_1.png](/assets/images/start/retraction_when_cut/deactive_retraction_when_cut_1.png =x400)

![deactive_retraction_when_cut_2.png](/assets/images/start/retraction_when_cut/deactive_retraction_when_cut_2.png =x400)


### AMS - Disable unloading and flushing to save filaments

Some comment sections mention this option, but this is completely different from the option above.

If you are using a BMCU but always connected to multiple identical filaments just for auto refill, and you don't want it flushing at the beginning and end of each print, you can do this.

https://wiki.bambulab.com/en/ams/manual/ams-not-unloading-to-save-filament

Please note that, as with the official AMS, if you do this, the BMCU may also remain active instead of into standby mode, which may prevent you from switching between filament types and colours, so in general it is not recommended to turn this option on.