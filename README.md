# Official Nord 4 Kerenel Source
[OnePlusOSS](https://github.com/OnePlusOSS/kernel_manifest)

# Requirement:
------
* Bootloader Unlocked

* 6.1.75 Kernel based
 
* Little Brain ☺️
------

## Required Modules

* [Susfs for KernelSU](https://github.com/sidex15/ksu_module_susfs)

------
> [!CAUTION]
> Do **NOT** install modules during **root-preserving updates**!
>
> Remember to press **Volume Down** when installing the module!
>
> If you have enabled the `ZRAM` algorithm, make sure to install the `ZRAM` module
> **before rebooting** after flashing with `Anykernel3`. You may need to adjust some parameters manually.The 5.10 kernel is not supported `ZRAM` , as the `zram.ko` module path could not be found.However, the generated ``Anykernel3`` is still usable.

------


# How TO :
------
### Flash Kernel :

* Use [Kernel Flasher](https://github.com/fatalcoder524/KernelFlasher)

### Update Your Device Without Losing Root Access  

#### Method 1: For Magisk or KernelSU (LKM) Users  
If you're rooted using Magisk or KernelSU, follow these steps to update while preserving root:  

1. Download the full OTA update for your device.  
2. Install the update using Local Update (via your device’s system updater).  
3. Before restarting:  
   - Open Magisk/KernelSU.  
   - Tap "Install" → "Install to Inactive Slot (After OTA)".  
4. Once done, return to the updater and tap "Restart".  

Your device will reboot with the update applied and root access intact.  

#### Method 2: For GKI Kernel Users (Custom Kernel with SUFS)  
If you’re using a patched GKI kernel (e.g., SUFS-modified kernel), follow these steps:  

1. Download the full OTA update.  
2. Install the update via Local Update (in the system updater).  
3. Before restarting:  
   - Open Kernel Flasher.  
   - Flash AnyKernel3 (AK3) to the inactive slot.  
   - Do not select any additional options after flashing.  
4. Return to the updater and tap "Restart".  

Your device will boot into the updated system with the custom kernel and root preserved.  

## Important Notes:  
* Always back up your data before updating.  
* Ensure you’re using the full OTA, not an incremental update.  
* If using Magisk Delta or a custom Magisk fork, the steps may vary slightly.  

This ensures a smooth update process without losing root or kernel modifications.

------

## Features

Features:  
[+] SukiSU Ultra 
[+] SUSFS CI
[+] VFS HOOK  
[+] Magic Mount Support KPM 
[+] BBR Support
[+] ZRAM


# Thanks to :

* [SukiSU](https://github.com/SukiSU-Ultra/SukiSU-Ultra)

PS. I won't be responsible for anything caused by this. Do at your own risk!