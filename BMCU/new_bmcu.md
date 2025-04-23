---
title: Just got a BMCU / How to start using BMCU
description: 
published: true
date: 2025-04-23T15:18:23.614Z
tags: 
editor: markdown
dateCreated: 2025-03-31T11:20:11.177Z
---

todo

drafts

do not hot plug / unplug

Known defects - some channels will always show the presence of filament

### If you are using BMCU-B and you found your 5way(AMS Lite Hub) pops up 
Like this:
![5_way_pop_up.gif](/assets/images/gif/5way_pop_up.gif =x300)

One of the solutions is as follows.
This option is recommended but not always required. If you are not experiencing problems with five-way it is usually not necessary to do this additionally.

This option is a separate setting for filaments, which means you will need to set it for all your filaments multiple times.

![deactive_retraction_when_cut_1.png](/assets/images/start/retraction_when_cut/deactive_retraction_when_cut_1.png =x300)

![deactive_retraction_when_cut_2.png](/assets/images/start/retraction_when_cut/deactive_retraction_when_cut_2.png =x300)


### AMS - Disable unloading and flushing to save filaments

Some comment sections mention this option, but this is completely different from the option above.

If you are using a BMCU but always connected to multiple identical filaments just for auto refill, and you don't want it flushing at the beginning and end of each print, you can do this.

https://wiki.bambulab.com/en/ams/manual/ams-not-unloading-to-save-filament

Please note that, as with the official AMS, if you do this, the BMCU may also remain active instead of into standby mode, which may prevent you from switching between filament types and colours, so in general it is not recommended to turn this option on.