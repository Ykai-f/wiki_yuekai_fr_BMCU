# 📂 BMCU-C Firmware v0019

This folder contains the **v0019 universal firmware** for **all BMCU-C boards**, including the upcoming dual microswitch Hall sensor version.

> 🔧 "**Universal**" means it works across all A1/P1/X1 printers, as long as you’re using a **370 motor and Hall-based buffer**.  
> The choice of sub-board does not matter; for P1, just ensure the pipe length is configured correctly to choose **internal** or **external** version.  
> A1 is configured as internal by default and does not require adjustment.

---

## 🔤 Firmware Naming (A/B/C/D)

The files named `BMCU-C-0019-P-X-Series-Int/Ext-Hub-A/B/C/D` are specifically for **P1 series**:

- Choose `Int` or `Ext` version according to your Hub location.
- The suffix `A`, `B`, `C`, `D` determines the printer’s ability to recognize up to 4 devices.
- For A1, you can **directly flash `BMCU-C-0019-A Series Printer.bin`** without concern.

---

## 🔧 Practical Examples

Here are some common usage scenarios and the corresponding firmware to flash:

- 🟢 **For A1 mini**:  
  Flash `BMCU-C-0019-A Series Printer.bin`

- 🟢 **For A1**:  
  Flash `BMCU-C-0019-A Series Printer.bin`

- 🟢 **For P1S using a single BMCU with external 5-way hub**:  
  Flash `BMCU-C-0019-P-X-Series-Ext-Hub-A.bin`

- 🟢 **For P1S using two BMCUs with external 5-way hubs**:  
  - Flash `BMCU-C-0019-P-X-Series-Ext-Hub-A.bin` on BMCU #1  
  - Flash `BMCU-C-0019-P-X-Series-Ext-Hub-B.bin` on BMCU #2

## 🔧 What's New in v0019 (Compared to v0013)

- ✅ **16-color support** for P1/X1 printers (requires flashing the new firmware)
- 🛠️ Fixed the issue where **filament info could not be saved** on the latest P1 firmware (`00.01.06.62`) and slicing software (`2.1.1.52`)
- ⚙️ Refined online channel logic to prevent incorrect status detection in edge cases
- ⚡ Improved motor control: separate logic for high and low voltage scenarios

---

## 💡 Changes Compared to Previous v0013 (Anti-Overheat Light Optimization)

- 🌙 Mainboard LED Behavior:
  - Red breathing light when not connected to printer
  - White breathing light when working normally
- 🔅 Further reduced LED brightness for buffer and mainboard to prevent overheating
- 🔁 Ejection behavior revised: removed A1-specific retraction control for broader compatibility

---

If you have any questions or suggestions, feel free to reach out to the community or our support group.  
We’re committed to continuously improving the BMCU firmware experience.

---
