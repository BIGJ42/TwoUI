# TwoUI

**TwoUI** is a One UI clone built on top of LineageOS, enhanced with Magisk for seamless integration of Samsung One UI features. It brings the sleek design and functionality of Samsung's One UI to your device running LineageOS by leveraging Magisk modules to enable One UI launcher, apps, device spoofing (to Samsung Galaxy S25 Ultra), and much more.

---

## Features

- **One UI Home Launcher** enabled via Magisk
- Preinstalled One UI system apps
- Device spoofing as Samsung Galaxy S25 Ultra (for app compatibility and enhanced features)
- Additional tweaks and enhancements to mimic One UI experience
- Root access and systemless modifications through Magisk
- Play integrity fix for google play

---

## Modules Used
All modules used are owned by their respective Creators.
reiryuki: One Ui Core and Home Modules
@VKsUpdates: One UI Experience Module
chiteroman: Play Integrity Fix Module

## Requirements

- A device compatible with GSIs
- Magisk installed on your device
- Basic knowledge of ADB and fastboot

---

## Installation Instructions

### 1. Patch your `boot.img` with Magisk

To enable Magisk (and so OneUI features) and root access, you need to patch your device's `boot.img`:

1. Download the `boot.img` file from your current ROM or device firmware.
2. Transfer the `boot.img` to your device.
3. Open the [Magisk app](https://github.com/topjohnwu/Magisk/releases/tag/v29.0) on your device.
4. Select **Install** > **Install** > **Select and Patch a File**.
5. Choose the `boot.img` file you transferred.
6. Magisk will patch the image and save it as `magisk_patched.img` in your device's `Download` folder.
7. Transfer `magisk_patched.img` back to your PC.

### 2. Flash the patched boot image

1. Reboot your device into recovery/bootloader/fastboot mode.
2. Flash the patched image with the following command:

   ```bash
   fastboot flash boot magisk_patched.img
'
Or Flash in TWRP as Boot Image [DynaPatch Needed](https://t.me/dev_yilliee/215).
