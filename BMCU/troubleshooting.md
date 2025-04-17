---
title: Troubleshooting
description: 
published: true
date: 2025-04-17T19:45:00.978Z
tags: 
editor: markdown
dateCreated: 2025-02-25T12:08:58.045Z
---

### 1️⃣ Printer Cannot Recognize AMS, or Main Board Shows Red Light 🚨

<details>
  <summary>Click to expend</summary>
After connecting to the printer the motherboard shows a red light meaning that the BMCU and printer communication is **not** established, however power is successfully supplied to the BMCU.
If you make your own data cable, check first if the AB wire sequence is wrong.

Then check for possible PCB issues, such as:
- Loose solder joints on components
- Faulty communication wiring (e.g., missing resistors in communication lines)
- Incorrect chip orientation or poor soldering causing virtual connections
  
  
Worst case scenario, the AMS connector board or printer motherboard is damaged. Or the 75176 chip on BMCU is damaged.
</details>


### 2️⃣ No Material Inserted, but System Shows Material Present (Or filament led keeps on) 📏
<details>
  <summary>Click to expand</summary>

#### 🧩 Issue Description  
The system reports that filament is present even when no material has been inserted. This can manifest as:

- The filament detection indicator (LED) remaining **ON**
- In AMS menu display filament always present in a certain channel

---

#### 🔍 Cause  
This behavior is a **known limitation** of the BMCU design, which relies on an optical sensor aligned with a narrow structural hole. The sensor detects filament presence when the beam is interrupted.

False positives (i.e., filament always detected) may occur due to:

- Slight height inconsistency of the photoelectric sensor at the factory 
- Slight height inconsistency of the photoelectric sensor at the time of soldering 
- Shape deviation at the time of printing of the detection aperture 
- Debris or dust blocking the optical path

The steel ball version is designed to reduce the chance of this problem, but we have noticed that some users even with the steel ball version still encounter this situation.

---

#### ✅ Why It Usually Doesn't Affect Printing  
This issue is generally **non-critical**. A false positive — where filament is always reported as present — is much less disruptive than a false negative, which might prematurely pause a print.

Additionally, the firmware includes a **secondary safeguard**:  
It monitors filament movement within the extruder. If no filament is actually being pushed through, the system will trigger a pause automatically, ensuring job protection.

---

#### 🛠️ Optional Improvements  
If you'd like to improve sensor reliability, you may consider:

- Gently cleaning the optical hole and slider using a precision tool to remove dust or filament residue  
- Slightly enlarging the detection hole with a micro drill bit (1.2 mm recommended)  
  ⚠️ *Do not exceed 1.2 mm*, or the sensor may incorrectly report "no filament" due to too easy for light passing through   
- Re-soldering or re-aligning the optical sensor if visibly misaligned  
- If you are using non-steel ball version, you can try upgrading -> need reprint almost everything and completely disassemble the BMG gear, and purchase additional parts
  
⚠️ Impact on Auto Refilling Function
This issue can negatively affect the auto refilling feature. For example:

- Suppose the filament detection on Channel 1 is faulty and always reports filament as present.
- You are about to run out of filament on Channel 1
- You have set up Channel 2 with the exact same material, expecting the printer to automatically refill from it.

However, when the filament on Channel 1 runs out, the printer may fail to recognize the absence correctly. As a result, it might trigger a filament jam error instead of recognizing a normal runout and switching to Channel 2.

If you're using the BMCU mainly for auto refilling purposes, we recommend the following setup:

- Connect the spool that is likely to run out to a channel where filament detection is working correctly in this exemple channel 2.
- Connect the backup spool (with enough material) to the channel affected by this issue in this case channel 1.

This setup will ensure that when the primary spool is depleted, the system can detect it accurately and trigger the refilling process as expected.

---

> 🔧 **Note:** Due to mechanical and manufacturing tolerances, this issue affects many BMCU units to some extent. In most cases, it does **not** impair normal printing operations.

</details>



### 3️⃣ Material Feeds In and Then Retreats, Unable to Continue Feeding

<details>
  <summary>Click to expend</summary>
  Solution:
  This issue is often caused by:
  - Missing radial magnet
  - Magnet holder not rotating with the shaft
  - Ejected magnetic disc not installed properly

  🛠️ Fixes:
  - Use a correctly sized and oriented radial magnet (6×2.5mm)
  - Check and ensure the AS5600 encoder chip is properly soldered
  - Test magnetic polarity: Two magnet surfaces should attract each other. If they repel when rotated 180°, it's the wrong orientation 🔄  
</details>


### 4️⃣ Device Manager Cannot Detect MainBoard or Downloader (USB to TTL) 

<details>
  <summary>Click to expend</summary>
🛠️ Troubleshooting Steps

  #### Verify Downloader Recognition

First, connect the USB-to-TTL downloader alone to your computer (without connecting to the mainboard).

- If it appears as a serial device (e.g., COMx) in Device Manager, the driver is properly installed.
- If no device appears, install the CH340 USB-to-Serial driver (commonly used in many USB-TTL modules).

#### Check for Short Circuits on the Mainboard

If the downloader is detected when connected alone, but disappears or disconnects when attached to the mainboard, this often indicates a short circuit, typically between 3.3V and GND.

Carefully inspect the circuitry around the CH32V microcontroller for any solder bridges or damaged components.

#### Ensure Correct Wire Connections

Double-check the DuPont wire order: TX ↔ RX, RX ↔ TX, GND ↔ GND, and 3.3V.


#### Disable USB Port Protection (if applicable)

On some PCs, aggressive USB port protection or antivirus software may prevent the downloader from being recognized.

Try switching to another USB port or temporarily disabling port protection if you're familiar with your system's settings.
</details>


### 5️⃣ Firmware Update Failed, PC Recognizes Device but Cannot Unlock or Flash Firmware

<details>
  <summary>Click to expend</summary>
  Solution:
  https://wiki.yuekai.fr/BMCU/BMCU_Tutorial/BMCU_Flashing#h-5-flash-the-firmware
</details>


### 6️⃣ Feeder Motor Spins but Doesn't Feed Material Properly

<details>
  <summary>Click to expend</summary>
  Solution:
  - Triangular gear may be too tight, preventing engagement.
  - Precision errors in external parts may cause jamming.  
</details>


### 7️⃣ Feeder Makes Loud Noise

<details>
  <summary>Click to expend</summary>
  Solution:
  - Check if screws are pressing against the motor shaft, causing friction.
  - Noise during feeding may be due to gear skipping, which is unavoidable.
  - Apply lubricant to reduce noise from misaligned gears.  
</details>


### 8️⃣ Waste Material Inserted, Indicator Light On, but Printer Doesn't Detect It

<details>
  <summary>Click to expend</summary>
  Solution:
  - Ensure the magnet is installed; it won't be recognized otherwise.
  - After installing the magnet, restart the device for detection.
  - Check for loose PH2.0 socket connections or broken ribbon cables.  
</details>


### 9️⃣ Abnormal Indicator Light Behavior When Cover is Not Installed

<details>
  <summary>Click to expend</summary>
  Solution:
  - Incorrect PH2.0 wiring, requires reversed 10-pin 80mm cable.
  - Check for loose socket connections.
  - Short circuits on the secondary board (e.g., resistor/capacitor bridging).  
</details>
