---
title: For Developers
description: 
published: true
date: 2025-05-09T00:16:54.917Z
tags: 
editor: markdown
dateCreated: 2025-05-09T00:03:29.178Z
---

# Building and Exploring the Source Code

If you would like to study or compile the BMCU source code, we recommend using `Visual Studio Code` with the `PlatformIO` extension. 
The recommended folder structure is as follows: 
```
BMCU/
├── platformio.ini
└── src/
    ├── main.cpp
    ├── main.h
    ├── motor_control.cpp
    ├── motor_control.h
    └── ..............

```

📄 platformio.ini Example

```
; PlatformIO Project Configuration File
;
;   Build options: build flags, source filter
;   Upload options: custom upload port, speed and extra flags
;   Library options: dependencies, extra library storages
;   Advanced options: extra scripting
;
; Please visit documentation for the other options and examples
; https://docs.platformio.org/page/projectconf.html

[env:genericCH32V203C8T6]
platform = https://github.com/Community-PIO-CH32V/platform-ch32v.git

board = genericCH32V203C8T6
framework = arduino
lib_deps = 
	robtillaart/CRC@^1.0.3
build_flags= -D SYSCLK_FREQ_144MHz_HSI=144000000
```