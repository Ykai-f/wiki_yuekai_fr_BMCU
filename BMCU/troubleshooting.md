---
title: Troubleshooting
description: 
published: true
date: 2025-03-10T14:40:18.032Z
tags: 
editor: markdown
dateCreated: 2025-02-25T12:08:58.045Z
---

<h3>1️⃣ Printer Cannot Recognize AMS, or Main Board Shows Red Light 🚨</h3>

<details>
  <summary>Click to expend</summary>
  <b>Solution:</b><br>
  This issue is often caused by incorrect AB wire sequence in connecting cable. Try swapping the connections. If the problem persists, check for possible PCB issues, such as:<br><br>
  - Loose solder joints on components<br>
  - Faulty communication wiring (e.g., missing resistors in communication lines)<br>
  - Incorrect chip orientation or poor soldering causing virtual connections 
</details>

<hr>

<h3>2️⃣ No Material Inserted, but System Shows Material Present 📏</h3>

<details>
  <summary>Click to expend</summary>
  Even when there's no material, the system still detects it, the waste material recognition light is on, or material feeding is unstable.<br><br>
  
  <b>Solution:</b><br>
  This is commonly due to:<br>
  - Misaligned optical sensor on old model parts<br>
  - Incorrect feed channel width<br>
  - Uneven soldering between the optical sensor and PCB <br><br>

  <b>🛠️ Fixes:</b><br>
  - Upgrade to a <b>newer optical module</b> 🔄<br>
  - Re-solder the optical sensor 🔩<br>
  - Adjust the feeding module manually for better alignment ⚙️  
</details>

<hr>

<h3>3️⃣ Material Feeds In and Then Retreats, Unable to Continue Feeding</h3>

<details>
  <summary>Click to expend</summary>
  <b>Solution:</b><br>
  This issue is often caused by:<br>
  - <b>Missing radial magnet</b><br>
  - <b>Magnet holder not rotating with the shaft</b><br>
  - <b>Ejected magnetic disc not installed properly</b><br><br>

  <b>🛠️ Fixes:</b><br>
  - Use a <b>correctly sized and oriented radial magnet (6×2.5mm)</b><br>
  - Check and <b>ensure the AS5600 encoder chip is properly soldered</b><br>
  - <b>Test magnetic polarity</b>: Two magnet surfaces should <b>attract</b> each other. If they <b>repel</b> when rotated 180°, it's the wrong orientation 🔄  
</details>

<hr>

<h3>4️⃣ Firmware Not Recognized, Device Manager Cannot Detect Downloader (USB to TTL)</h3>

<details>
  <summary>Click to expend</summary>
  <b>Solution:</b><br>
  - Check if the mainboard is short-circuited (3.3V to GND).<br>
  - Ensure DuPont wires are connected in the correct order.<br>
  - Some downloads may trigger PC protection, preventing detection.  
</details>

<hr>

<h3>5️⃣ Firmware Update Failed, PC Recognizes Device but Cannot Unlock or Flash Firmware</h3>

<details>
  <summary>Click to expend</summary>
  <b>Solution:</b><br>
  - Check for incorrect soldering of the main control chip.<br>
  - Look for virtual solder joints or short circuits.<br>
  - Incorrect DuPont wire order may cause issues.<br>
  - If C board prompts unlock failure, retry multiple times.  
</details>

<hr>

<h3>6️⃣ Feeder Motor Spins but Doesn't Feed Material Properly</h3>

<details>
  <summary>Click to expend</summary>
  <b>Solution:</b><br>
  - Triangular gear may be too tight, preventing engagement.<br>
  - Precision errors in external parts may cause jamming.  
</details>

<hr>

<h3>7️⃣ Feeder Makes Loud Noise</h3>

<details>
  <summary>Click to expend</summary>
  <b>Solution:</b><br>
  - Check if screws are pressing against the motor shaft, causing friction.<br>
  - Noise during feeding may be due to gear skipping, which is unavoidable.<br>
  - Apply lubricant to reduce noise from misaligned gears.  
</details>

<hr>

<h3>8️⃣ Waste Material Inserted, Indicator Light On, but Printer Doesn't Detect It</h3>

<details>
  <summary>Click to expend</summary>
  <b>Solution:</b><br>
  - Ensure the <b>magnet is installed</b>; it won't be recognized otherwise.<br>
  - After installing the magnet, <b>restart the device</b> for detection.<br>
  - Check for <b>loose PH2.0 socket connections</b> or broken ribbon cables.  
</details>

<hr>

<h3>9️⃣ Abnormal Indicator Light Behavior When Cover is Not Installed</h3>

<details>
  <summary>Click to expend</summary>
  <b>Solution:</b><br>
  - <b>Incorrect PH2.0 wiring</b>, requires <b>reversed 10-pin 80mm cable</b>.<br>
  - Check for <b>loose socket connections</b>.<br>
  - <b>Short circuits on the secondary board</b> (e.g., resistor/capacitor bridging).  
</details>
