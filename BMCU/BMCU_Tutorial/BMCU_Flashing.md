---
title: BMCU_Flashing
description: 
published: true
date: 2025-03-03T22:13:39.089Z
tags: 
editor: markdown
dateCreated: 2025-01-29T10:53:40.895Z
---

# **BMCU Flashing Tutorial (Serial Port Flashing)**

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

## **Flashing Tutorial**

1. **Connect the BMCU Mainboard and USB Serial Tool According to the Wiring Instructions**  
   - <span style="color:red">**⚠️ DO NOT CONNECT THE BMCU TO THE PRINTER DURING WHOLE PROCESS!!!!!!** 🚨  
 ![1.png](/assets/images/bmcu_flashing/1.png)  
 
 2. **Connect the USB Serial Tool to the Computer**  
   - The computer should automatically recognize the serial port.  
   - Refer to the diagram for guidance, but note that **your serial port number may differ** from the one shown in the image.  
![2.png](/assets/images/bmcu_flashing/2.png)
![3.png](/assets/images/bmcu_flashing/3.png)

3. **Press and Hold the B Button**  
   - **Use your left hand** to **press and hold the B button** (**Do not release it!**).  
   - **With your right hand**, press the **R button** once, then release it.  
   - **⚠️ The B button should ideally remain pressed throughout the process.**
![4.png](/assets/images/bmcu_flashing/4.png)
  
  If it goes well, you should see the word <font color="red">”unlocked“</font> in red in the software
  
>   If it keeps failing, try swapping the T and R wires on the motherboard, which is the case with some chips.
{.is-warning}

  
 4. **Open the WCHISPTOOL Software**  
   - Select the **corresponding MCU series**, **model**, **download method**, and check the necessary **download configuration** options.  
   - Follow the steps below to proceed.  
   - **If the message** `"Unlock read/write protection successful!"` **appears, the operation was successful.** ✅  
![5.png](/assets/images/bmcu_flashing/5.png)
  
  
5. **Click the Download Button**  
   - **Be patient** while the download process completes.  
   - If the download is **successful**, it should look like the reference image.  
   - **⚠️ If the download fails, try selecting 115200 baud rate.**  
![6.png](/assets/images/bmcu_flashing/6.png)

6. **Press the R Button**  
   - At this point, **press the R button**, and the **BMCU mainboard's red LED should light up**.  
   - 🎉 **Congratulations! The firmware flashing is successful!** 🎉  

  

## **Troubleshooting**
- Ensure the baud rate is set to **115200**.  
- Check the **stability of the Dupont wire connections**.  
- **Each time you download, you must click "Touch Protection" before proceeding.**  
  
# Testing  

<span style="color:red;font-size: 20px"><b> ⚠️⚠️⚠️Avoid hot plugging and unplugging the motherboard and printer cables.⚠️⚠️⚠️</span></b>
The right approach（just in case you are not sure what to do):
1. Power off the printer
1. Connect the BMCU to the printer
1. Switch on the printer power
1. You should see AMS appear in the consumables option, even if you have not inserted consumables, it may show that consumables are present in some channels (known bug)
1. Power off the printer
1. Disconnect the BMCU cable
