---
title: BMCU_Flashing
description: 
published: true
date: 2025-04-04T18:47:32.013Z
tags: 
editor: markdown
dateCreated: 2025-01-29T10:53:40.895Z
---

# **BMCU Flashing Tutorial (Serial Port Flashing)**


> If you did **not** solder the motherboard yourself, flashing is usually **not required**. Unless you want to upgrade the firmware.  
> All motherboards shipped from me come **pre-flashed** with firmware.  

## ⚠️ **WARNING**  
<span style="color:red">🔥 **Before flashing, ensure there are no soldering issues!!!! Check for power short circuits!!!!** 🔥  
🔥 **Before flashing, ensure there are no soldering issues!!!! Check for power short circuits!!!!** 🔥  
🔥 **Before flashing, ensure there are no soldering issues!!!! Check for power short circuits!!!!** 🔥  

---

## **Required Tools**
1. **Multiple Dupont Wires** (To connect the flasher and the BMCU mainboard).  
2. **USB to Serial Adapter** 
3. **Computer**.  
4. **Software: WCHISPTool**  
[wchisptool-v3.3.7z](/assets/files/wchisptool-v3.3.7z)

## 🪛 **Step-by-Step Flashing Guide**

### 1. **Connect the BMCU Mainboard and USB Serial Tool**

- Connect wires according to the wiring instructions.
- ⚠️ **DO NOT connect the BMCU to the printer during the entire process!**  
![1.png](/assets/images/bmcu_flashing/1.png)

---

### 2. **Connect the USB Serial Tool to Your PC**

- Your computer should recognize the serial port automatically.
- The COM port number might differ from the example in the image.  
![2.png](/assets/images/bmcu_flashing/2.png)  
![3.png](/assets/images/bmcu_flashing/3.png)

---
  
  ### 3. **Configure WCHISPTool Settings**

Open the `WCHISPTool` software and set the following options:

- **Chip Model:** `CH32V203`  
- **Download Type:** `SerialPort`  
- **DI – Baud Rate:** `1M`  
- **SerialPort:** Auto-detected (your COM port)  
- **User File:** Choose the firmware `.bin` file (available from our wiki)  

![5.png](/assets/images/bmcu_flashing/5.png)

---

### 4. **Unlock the Chip Protection**

This is a **critical step** before flashing the firmware.

#### ✅ Recommended Method:

1. **Hold down the B button** (do **not** release it throughout).
2. While holding B, **briefly press the R button** once.
3. While **still holding B**, click the **"Remove Protect"** button in the WCHISPTool software.

If successful, you’ll see a red **“Unlocked”** message in the tool.  
![4.png](/assets/images/bmcu_flashing/4.png)

> ⚠️ If it keeps failing:
> - First, try again using the same button sequence carefully.
> - Second, **double-click the “Download” button** to force the chip into response mode, then try "Remove Protect" again.
> - （Rare but indeed some chips will perform like this) try **swapping the TX and RX wires** (i.e., TX-to-TX and RX-to-RX instead of cross).

---



### 5. **Flash the Firmware**

Click the **Download** button.

- Be patient during the process.
- If flashing is successful, it should look like this:  
![6.png](/assets/images/bmcu_flashing/6.png)

#### ⚠️ If Flashing Fails:

- Try **pressing and holding the B button** while clicking “Download”.
- Alternatively, try changing the **baud rate to 115200**.
- In rare cases, try **reversing TX and RX** (TX-to-TX, RX-to-RX) if not already done.

---

### 6. **Reboot the Board**

- Press the **R button** once.
- The **red LED on the mainboard** should now light up.
- 🎉 **Congratulations! Firmware flashing is complete!** 🎉

---

## 📬 Help Us Improve

If you successfully flashed the firmware using the **English version** of WCHISPTool,  
we’d love to include a screenshot in our wiki to help others – feel free to send it over!

Let us know if you encounter any issues.
  

## **Troubleshooting**
- Try Baud Rate **115200**.   
  
# Testing  

<span style="color:red;font-size: 20px"><b> ⚠️⚠️⚠️Avoid hot plugging and unplugging the motherboard and printer cables.⚠️⚠️⚠️</span></b>
The right approach（just in case you are not sure what to do):
1. Power off the printer
1. Connect the BMCU to the printer
1. Switch on the printer power
1. You should see AMS appear in the consumables option, even if you have not inserted consumables, it may show that consumables are present in some channels (known bug)
1. Power off the printer
1. Disconnect the BMCU cable
