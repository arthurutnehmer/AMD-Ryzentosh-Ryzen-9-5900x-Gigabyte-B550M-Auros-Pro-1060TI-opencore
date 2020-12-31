[![macOS version](https://img.shields.io/badge/macOS-10.13.6%20(17G14042)-informational.svg)](https://www.apple.com/macos) [![OpenCore version](https://img.shields.io/badge/OpenCore-0.6.4-informational.svg)](https://github.com/acidanthera/OpenCorePkg) 

# AMD-Ryzentosh Ryzen 9 5900x Gigabyte B550M Auros Pro Nvidia 1060Ti

OpenCore 0.6.3 configuration  


## Hardware

| Type                 | Name                              |
|----------------------|-----------------------------------|
| CPU                  | AMD Ryzen 9 5900x                 |
| MB                   | Gigabyte B550M Auros Pro.         |
| Audio                | Realtek                           |
| GPU                  | NVIDIA GeForce GTX 1060 6GB       |
| RAM                  | 16G 3933Mhz DDR4 (8G * 2)         |
| Ethernet             | Realtek Gigabit Gaming Network    |
| Disk                 | Sabrent Rocket 4.0 1TB            |



![ScreenShot](https://i.imgur.com/g2ltthw.png)
![ScreenShot](https://i.imgur.com/X05yVe8.png)

## ACPI
- [SSDT] SSDT-CPUR.aml
- [SSDT] SSDT-EC-USBX-DESKTOP.aml
- [SSDT] SSDT-EC0.aml

## Patches & Kexts
 - [[Patch] AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
 - [[Kext] VirtualSMC](https://github.com/acidanthera/VirtualSMC)
 - [[Kext] Lilu](https://github.com/acidanthera/Lilu)
 - [[Kext] WhateverGreen](https://github.com/acidanthera/WhateverGreen)
 - [[Kext] AppleALC](https://github.com/acidanthera/AppleALC)
 - [Kext] AppleMCEReporterDisabler
 - [Kext] AMDRyzenCPUPowerManagement
 - [Kext] RealtekRTL8111
 - [Kext] USBInjectAll.kext



## What's working:

* Ethernet (Realtek Gigabit Gaming Network Connection)
* Display Port audio (though no volume control)
* Audio output
* Sleep
* iCloud, iMessage, Facetime
* Front USB ports are working
* Back USB ports are working
* Graphics
* FileVault
* Docker
* Adobe Products (Photoshop, XD)

## What's not working:
* Microphone input 
* Hardware Virtualization (VirtualBox is working fine, but Parallels isn't)
