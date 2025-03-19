---
title: BMCU Assembling
description: 
published: true
date: 2025-03-19T10:11:16.963Z
tags: 
editor: markdown
dateCreated: 2025-01-28T14:28:43.841Z
---

# BMCU Assembling
> <span style="color:red; font-size:30px;"><b>⚠️WARNING</b></span>
> <span style="color:red; font-size:25px;"><b>Do not hot-plug or unplug the connection cable between the BMCU and the printer while the printer is powered on. -> Risk of damage to the BMCU motherboard</b></span>
{.is-warning}

> You may receive a different version of the BMCU motherboard, or download a different version of the stl model, please check before printing and assembling
{.is-warning}



## Version & author
* v1.1&v1.31
* 130 Improved shell version
* Editor: 山竹

## Step 1: Testing the PCB Hardware


1. **Ensure Successful Firmware Burning for the BMCU Main Board (Firmware V0.2)**  
   - Use a USB-to-TTL burner to power the main board. The red indicator light should turn on.  
   - Connect the printer using an MX3.0 4-pin cable. The main board's blue indicator light should turn on.

2. **Verify the Functionality of the Secondary Board**  
   - Power the secondary board via USB. When connected to the main board:  
     - **RGB Lights:**  
       - The RGB light on the secondary board should show **blue** (port 1 is blue, ports 2, 3, 4 are off).  
       - The light flashing is considered normal.  
     - **Photoelectric Indicators:**  
       - The two photoelectric indicator lights should remain off under normal conditions.  
       - When the photoelectric sensors detect obstruction, the corresponding rear indicator light should turn on.  
       - For material detection:  
         - **RGB Light Behavior:**  
           - When feeding, the RGB light should turn **blue**.  
           - When a material jam occurs, the RGB light should turn **red**.  
     - When powered by a `Bambulab` printer:  
       - The RGB lights on both the main and secondary boards should remain **blue**.  
       - The two photoelectric indicator lights should remain off unless obstruction is detected, in which case the corresponding rear indicator lights should turn on.  
       - The **RGB lights** should consistently remain **blue**.

3. **Ensure Proper Communication Between the Main Board, Secondary Board, and Printer**  
   - When the main board is connected to the printer, the printer's **consumable menu** should display the **AMS option**.  
   - When the photoelectric sensors are obstructed, the **consumable status** should update to reflect the material detected.
   
## Step 2: Mechanical Assembly part 1 - Feeder/extruder, needs to be repeated 4 times

1. **Print the Complete Feeder Housing Set**  
   - Print the feeder housing according to the provided model.  
   - This tutorial is based on the following model:  
     [https://makerworld.com.cn/models/741793](https://makerworld.com.cn/models/741793) (**Modified by 青铜板子cn**).  
<br>
2. **Attach the Pneumatic Fitting (PC4-M6)**  
   - Screw the **PC4-M6 pneumatic fitting** into the buffer assembly.  
   - **Caution:** Ensure it is screwed in straight to avoid misalignment.
   ![bmcu_installation_2.2.jpg](/bmcu_installation_2.2.jpg =x250)
   
3. **Assemble the Spring and the 62B Axle Sleeve**  
   - Take one **large spring** (0.5 × 6 × 10mm) and a **62B axle sleeve**.  
   - Assemble them as shown in the diagram below:  
	![bmcu_installation_2.3.jpg](/bmcu_photo/bmcu_installation_2.3.jpg =x250)

4. **Compress the Spring and Snap it into the Base Housing**  
	![bmcu_installation_2.4.1.jpg](/bmcu_photo/bmcu_installation_2.4.1.jpg =x250)
	![bmcu_installation_2.4.2.jpg](/bmcu_photo/bmcu_installation_2.4.2.jpg =x250)


5. **Ensure the Components Move Freely** 
	![bmcu_installation_2.5.jpg](/bmcu_photo/bmcu_installation_2.5.jpg =x250)

6. **Assemble the Gear Structure**  
   - Take two **small gears (Gear 182A)** and one **short axle (2 × 10mm)**.  
   - Assemble them as shown in the diagram.  
   - Ensure the protruding sections on both sides of the axle are of equal length for proper alignment.  
	![bmcu_installation_2.6.jpg](/bmcu_photo/bmcu_installation_2.6.jpg =x250)

7. **Assemble the Large Gear and Long Axle**  
   - Take a **large gear (Gear 242A)** and a **long axle (2 × 20mm)**.  
   - Assemble them to match the diagram, ensuring one end of the axle is pressed to the width indicated by the arrow in the diagram.  
   
	![bmcu_installation_2.7.1.jpg](/bmcu_photo/bmcu_installation_2.7.1.jpg =x250)

8. **Select Two Triangular Parts (Replaceable)** 
	![bmcu_installation_2.8.jpg](/bmcu_photo/bmcu_installation_2.8.jpg =x250)

9. **Assemble the Large Gear with the Triangular Parts**  
   - Attach the **large gear** to the **triangular parts** as shown in the diagram.  
   - **Important:** Pay close attention to the **orientation of the gear** to ensure correct assembly.  
	![bmcu_installation_2.9.jpg](/bmcu_photo/bmcu_installation_2.9.jpg =x250)

10. **Assemble the Remaining Small Gears and Secure the Components**  
    - Attach the remaining **two small gears** to the structure.  
    - Place the cover over the assembly and tighten it using **M2 × 8 self-tapping screws**.  
    - Ensure all screws are securely fastened to maintain stability.  
	![bmcu_installation_2.10.jpg](/bmcu_photo/bmcu_installation_2.10.jpg =x250)
  ![bmcu_triangle_done.png](/bmcu_triangle_done.png =x250)

11. **Insert Axle Sleeves**
   - Insert **5 white 62B axle sleeves** into the positions shown in the diagram.  
   - Ensure they are securely pressed into the **base and top covers**.
   ![bmcu_installation_2.11.jpg](/bmcu_photo/bmcu_installation_2.11.jpg =x250)

12. **Prepare BMG Extrusion Components**
> A word of caution: please handle the combination of BMG gear set, D5*2 shaft and bearings with care, as the fit of the gears and shafts is sometimes very tight, and if it unfortunately gets stuck, it is very difficult to get it out again
{.is-warning}

   - Gather the following parts:  
     - **Extrusion wheel with <font color="red">screw hole</font> !!!!!! IMPORTANT**  
     - **Black set screw**  
     - **One thick axle (5 × 22mm)**  
     - **Two bearings (MR85ZZ)**.
     ![bmcu_installation_2.12.jpg](/bmcu_photo/bmcu_installation_2.12.jpg =x250)
     
     

13. **Assemble the Extrusion Wheel**
   - Assemble as shown in the diagram, paying close attention to orientation.  
   - One end of the **thick axle** must be flush with the bearing (to allow a flat surface for the magnet).  
   - **Don’t forget** to install the black set screw.
   ![bmcu_installation_2.13.jpg](/bmcu_photo/bmcu_installation_2.13.jpg =x250)

14. **Place the Extrusion Structure**
   - Insert the **extrusion structure** into the **base housing**.
   ![bmcu_installation_2.14.jpg](/bmcu_photo/bmcu_installation_2.14.jpg =x250)

15. **Insert the Gear Group**
   - Place the **gear group** into the axle sleeves, ensuring the **screw side faces downward**, as shown in the diagram.
   ![bmcu_installation_2.15.jpg](/bmcu_photo/bmcu_installation_2.15.jpg =x250)

16. **Install Two Long Axles**
   - Prepare **two long axles (2 × 20mm)**.  
   - Insert them into the **62B axle sleeves**.  
   - Install two **20082B double-layer straight gears**, starting from **left to right**.
   
   ![bmcu_installation_2.16.jpg](/bmcu_photo/bmcu_installation_2.16.jpg =x250)
   <span style="color:red">Note in image : 
  The left-down arrow gear is placed first, 
  The right-up arrow gear is installed later</span>
   ![bmcu_installation_2.16.2.jpg](/bmcu_photo/bmcu_installation_2.16.2.jpg =x250)

17. **Assemble the Motor and Worm Gear**
   - Combine the **FF-130 motor** with the **682A worm gear**.  
   - Ensure the assembly is flush; misalignment can cause gear jamming.
   ![bmcu_installation_2.17.jpg](/bmcu_photo/bmcu_installation_2.17.jpg =x250)

18. **Insert Axle Sleeves into Cover Plate**
   - Snap the **62B axle sleeves** (white parts) into the **holes on the cover plate**, as shown in the diagram.
   ![bmcu_installation_2.18.jpg](/bmcu_photo/bmcu_installation_2.18.jpg =x250)
   ![bmcu_installation_2.18.2.jpg](/bmcu_photo/bmcu_installation_2.18.2.jpg =x250)

19. **Attach Motor Cover Plate**
   - Fix the motor cover plate with **two M2 × 4 flat-head screws**.
   ![bmcu_installation_2.19.jpg](/bmcu_photo/bmcu_installation_2.19.jpg =x250)

20. **Solder Motor Wires**
   - Solder the connection wires to the motor.  
     - **Red dot** indicates the **positive terminal**.
     ![bmcu_installation_2.20.jpg](/bmcu_photo/bmcu_installation_2.20.jpg =x250)

21. **Install and Test the Motor**
   - Place the motor into the base housing and align it with the fixing slot.  
   - Power the motor with **3V-12V** to test if all gears rotate smoothly.
   <span style="color:red">Note in image : 
  Motor with sticker side down.
  The positive terminal should face downward for easier soldering later.
</span>

   ![bmcu_installation_2.21.jpg](/bmcu_photo/bmcu_installation_2.21.jpg =x250)

22. **Apply Lubricant and Secure the Cover**
   - Apply **lubricating grease** to the gears if desired.  
   - Place the cover plate on top and secure it with **M2 × 8 screws**.
   ![bmcu_installation_2.22.jpg](/bmcu_photo/bmcu_installation_2.22.jpg =x250)

23. **Insert the Replaceable Optical Sensing Module**
   - Place the **optical sensing module** into its designated slot.
   ![bmcu_installation_2.23.jpg](/bmcu_photo/bmcu_installation_2.23.jpg =x250)
   ![bmcu_installation_2.23.2.jpg](/bmcu_photo/bmcu_installation_2.23.2.jpg =x250)

24. **Thread Motor Wires Through Top Cover**
   - Thread the motor wires through the **slots on the top cover** and secure the cover in place.
   ![bmcu_installation_2.24.jpg](/bmcu_photo/bmcu_installation_2.24.jpg =x250)

25. **Insert Radial Magnet**
   - Insert a **radial magnet (6 × 2.5mm)** into the **red-circled hole on the top cover**.  
   - **Important:** Ensure smooth rotation and use the correct magnet size (not replaceable by a standard magnet).
   <span style="color:red; font-size:20px;"><b>Note: This magnet is used to detect the angle of rotation of the extrusion gear to obtain the material feed length.</b></span>
   ![bmcu_installation_2.25.jpg](/bmcu_photo/bmcu_installation_2.25.jpg =x250)

26. **Secure the Back Cover Screws**
   - Tighten the **five screws** (M2 × 8 self-tapping screws) on the **back cover**, as shown in the diagram.
   ![bmcu_installation_2.26.jpg](/bmcu_photo/bmcu_installation_2.26.jpg =x250)

27. **Install the Secondary Board**
   - Insert the secondary board and solder the motor wires (**observe polarity**).  
   - Secure the secondary board with **two M2 × 8 self-tapping screws**.
   ![bmcu_installation_2.27.jpg](/bmcu_photo/bmcu_installation_2.27.jpg =x250)

28. **Prepare Remaining Components**
   - Gather the following parts:  
     - Two **needle roller bearings**  
     - **BMG-supplied axle**  
     - **Non-perforated extrusion gear**  
     - **Printed wrench**.  
   - Assemble as shown in the diagram, ensuring the correct orientation.
   ![bmcu_installation_2.28.jpg](/bmcu_photo/bmcu_installation_2.28.jpg =x250)
   ![bmcu_installation_2.28.2.jpg](/bmcu_photo/bmcu_installation_2.28.2.jpg =x250)
   ![bmcu_installation_2.28.3.jpg](/bmcu_photo/bmcu_installation_2.28.3.jpg =x250)

29. **Place the Small Spring**
   - Place a **small spring (0.6 × 4 × 10mm)** in the position shown in the diagram.  
   - Snap the **wrench** into place, ensuring the spring is properly seated and compressed.
   ![bmcu_installation_2.29.jpg](/bmcu_photo/bmcu_installation_2.29.jpg =x250)

30. **Insert Short and Long Axles**
   - Use a **short axle (D2 × 10mm)** and a **long axle (D2 × 20mm)**.  
   - Insert the short axle first, followed by the long axle, through the wrench holes into the axle sleeve.  
   - Verify smooth movement when pressed and rotated.
   ![bmcu_installation_2.30.jpg](/bmcu_photo/bmcu_installation_2.30.jpg =x250)
   ![bmcu_installation_2.30.1.jpg](/bmcu_photo/bmcu_installation_2.30.1.jpg =x250)
   ![bmcu_installation_2.30.2.jpg](/bmcu_photo/bmcu_installation_2.30.2.jpg =x250)

31. **Secure the Final Cover**
   - Adjust the motor wires, place the final cover, and secure it with **four M2 × 8 self-tapping screws**.  
   - The **extrusion assembly** is now complete.
   ![bmcu_installation_2.31.jpg](/bmcu_photo/bmcu_installation_2.31.jpg =x250)

32. **Insert Transparent Material**
   - Insert transparent material into the **indicated holes**, ensuring it reaches the bottom, then cut it off.  
   - This will guide the **indicator light**.
   ![bmcu_installation_2.32.1.jpg](/bmcu_photo/bmcu_installation_2.32.1.jpg =x250)
   ![bmcu_installation_2.32.2.jpg](/bmcu_photo/bmcu_installation_2.32.2.jpg =x250)


## Step 3: Mechanical Assembly part 2 - Base Installation and Connections

1. **Connect the Feeders**
   - Insert the **PH2.0 10-pin male-to-male reverse cable** (80mm in length) into the feeder interface.
   ![3.1.jpg](/bmcu_photo/3.1.jpg =x250)

2. **Install Feeders onto the Top Cover**
   - Attach the feeder units to the **top cover of the base**, aligning them with the designated holes.  
   - Place the cables into the wire grooves to keep them organized.
![3.2.jpg](/bmcu_photo/3.2.jpg =x250)

3. **Secure Feeders**
   - From the **underside of the top cover**, tighten the screws (M2 × 8 self-tapping screws) at the red-circled positions.  
   - Repeat this process to secure all feeder units.
   ![3.3.jpg](/bmcu_photo/3.3.jpg =x250)

4. **Mount the Mainboard**
   - Install the **mainboard** onto the base, aligning it with the red-circled screw holes.  
   - Secure it with **M2 × 8 self-tapping screws**.
   ![3.4.jpg](/bmcu_photo/3.4.jpg =x250)

5. **Assemble the Base**
   - Combine the **base parts** as shown in the diagram.  
   - At the circled positions on the bottom of the base, secure it using **M3 × 14 self-tapping screws**.
   ![3.5.jpg](/bmcu_photo/3.5.jpg =x250)
   ![3.5.2.jpg](/bmcu_photo/3.5.2.jpg =x250)

6. **Connect Ribbon Cables and Finalize Assembly**
   - Insert the **ribbon cables** into their respective connectors.  
   - Place the **wire cover** over the cables and secure it at the circled positions with **M3 × 14 self-tapping screws**.
   
>    Before installing this cover, if you plan to install it on the printer immediately, please refer directly to the Mounting section
{.is-info}

   ![3.6.jpg](/bmcu_photo/3.6.jpg =x250)
   ![3.7.jpg](/bmcu_photo/3.7.jpg =x250)
   
## Done! :)
The **BMCU complete system** assembly is now finished.








  
  
  
  
  
  
  