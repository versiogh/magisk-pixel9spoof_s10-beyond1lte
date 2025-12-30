# Magisk Pixel 9 Pro Spoof Module for Samsung Galaxy S10 Exynos (SM-G973F beyond1lte)

## Overview
This Magisk module allows you to spoof a Pixel 9 Pro on a **Samsung Galaxy S10 Exynos (SM-G973F beyond1lte)** running custom ROMs (tested on LineageOS 16 and crDroid 12.0). It improves compatibility with Google apps that check the device (Play Store, SafetyNet, Netflix…).

**Key Features:**
- Permanent early fix for `ro.build.display.id` to prevent ROM overwrites
- Fixed Pixel 9 Pro fingerprint with per-boot randomized build number
- Full spoof of `ro.product.*` properties across all partitions
- SoC spoof: Google Tensor G4 (non-critical, consistency only)
- Clears Samsung/Knox flags (safe)
- Sets `ro.com.google.clientidbase` and `ro.oem_unlock_supported`

**Installation:**
1. Download the module ZIP from the [Releases](https://github.com/versiogh/magisk-pixel9spoof_s10-beyond1lte/tree/main).  
2. Check file permissions (for novice users):  
   - `/data/adb/modules/pixel_spoof/module.prop` → 0644  
   - `/data/adb/modules/pixel_spoof/post-fs-data.sh` → 0755  
   *(Use a root file explorer if unsure.)*  
3. Install via Magisk Manager → Modules → Install from file.  
4. Reboot.

**Tested On:**
- LineageOS 16 (Android 16)  
- crDroid 12.0 (based on LineageOS 16)

**Notes:**
- Backup your device before flashing.  
- Works on **Samsung Galaxy S10 Exynos (SM-G973F beyond1lte)**; results may vary on other devices.  
- Feedback and suggestions are welcome!

**License:**
This module is open-source under the MIT License. Feel free to fork, improve, or adapt it.

## Example Output

Here is an example of the spoofed properties observed via PowerShell on a Samsung Galaxy S10 Exynos (SM‑G973F beyond1lte):

![Spoofed Properties Screenshot](https://zupimages.net/up/25/01/4wyu.png)

As shown above, the module correctly applies Google Pixel 9 Pro identity and fingerprint values.
