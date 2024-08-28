# Hackintosh

[![OpenCore](https://img.shields.io/badge/OpenCore-0.8.8-blue.svg)](https://github.com/acidanthera/OpenCorePkg)
[![macOSver](https://img.shields.io/badge/macOS-13.4-brightgreen.svg)](https://support.apple.com/HT213843)

### ⚠️ Disclaimer

- Begin by using this EFI as a foundational starting point. Ensure you create your own EFI following the Dortania OpenCore Install Guide.
- Please note that this EFI may not always be updated to the latest version of OpenCore, particularly if there have been no significant changes.
- It is crucial to read this entire README before proceeding.

#####

![About This Mac](https://raw.githubusercontent.com/Hackoak/hackintosh/master/Ventura/Details/About%20This%20Mac_v.png)


### Latest info

**OS**: macOS Ventura 13.4 (22F66)
<br>
**OpenCore**: 0.8.8
<br>
**SMBIOS**: iMac18,1
<br>
**Release date**: 28/5/2023

# 🖥️ Hackintosh Specs

|Item|Description|
|-|:-------:|
|CPU|Intel Core i7 7700|
|Memory|2x 8Gb DDR4 2400Mhz|
|Storage|480GB SSD KINGSTON SA400S372480G |
|GPU|iGPU Intel HD Graphics 630 1536 MB|
|Ethernet|RTL8111/8168/8411 PCI Express Gigabit Ethernet|
|WLAN+Bluetooth|TP-Link Archer T2Ub Nano Ac600|
|Audio|Realtek ALC887 (0x0887)|
|Mobo|ASUS H110M-D|

### ✅️ What works</strong></summary>

- iGPU acceleration Intel HD 630
- Audio
- Bluetooth
- HDMI port
- Ethernet
- iMessage
- Virtualization (Android Emulator)

### ❌️ What doesn't work

- Sleep
- WIFI
- Airdrop (No natively compatible wifi adapter)


# MacOS Ventura
[![OpenCore](https://img.shields.io/badge/OpenCore-0.8.8-blue.svg)](https://github.com/acidanthera/OpenCorePkg)
[![macOSver](https://img.shields.io/badge/macOS-13.4-brightgreen.svg)](https://support.apple.com/HT213843)

**OS**: macOS Ventura 13.4 (22F66)
<br>
**OpenCore**: 0.8.8
<br>
**Release date**: 28/5/2023
<br>
<br>
![About This Mac](https://raw.githubusercontent.com/Hackoak/hackintosh/master/Ventura/Details/About%20This%20Mac_v.png)

# ⚙️ Setup

> [!CAUTION]
> This step is mandatory to get the device booting and get iGPU work

<details>
<summary><strong>⚒️ Pre installation</strong></summary>

1. Download the MacOs Installer image from Open core legacy patcher or anywhere else
2. Use the below command to flash it to USB
```bash
sudo /Applications/Install\ macOS\ Ventura.app/Contents/Resources/createinstallmedia --volume /Volumes/USB_Name
```
3. After completed Mount the USB EFI via Opencore legacy patcher or anything else
4. Copy the EFI under the `Ventura/EFI/Pre install EFI` path & paste under the USB EFI path and rename it to `Pre install EFI > EFI`
5. Boot the Hackintosh with USB
6. You will Notice the Graphics will not work after the setup let fix that in Post installation

#####

</details><details>
<summary><strong>✅ Post installation</strong></summary>

1. Once the Ventura initial Setup completed
2. Mount the System EFI  
3. Copy the EFI under the `Ventura/EFI/Post install EFI` path & paste under the System EFI path and rename it to `Post install EFI > EFI`
4. Open the [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools/releases) and load the System EFI `config.plist` file
5. Select `PlatformInfo` (PI) and click the `Generate` button near the `SystemProductName` it will generate the SMBIOS serial.
6. **IMPORTANT:** reminder that you need an **invalid serial!** to check copy and paste the second part saying `Serial: XXXXX..` in [Apple's Check Coverage Page](https://checkcoverage.apple.com/), if you get a red message saying "We're sorry, we're unable to check coverage for this serial number."
 then you're good to go! Otherwise, `Generate` again.
7. once you get the right serial number, click the Save button at top.
8. Restart and enjoy 🎉
⊖−⊟

</details>

##### 

# ✨ Status

- ☑︎  iGPU acceleration Intel HD 630
- ☑︎  Bluetooth
- ☑︎  Audio
- ☑︎  HDMI port
- ☑︎  Ethernet
- ☑︎  iServices
- ☑︎  Virtualization (Android Emulator)
- ⊖  WIFI
- ⊖  Airdrop (No natively compatible wifi adapter)

<!-- 
## Where to Buy

|Part|Link to Buy|
|-|:-------:|
|Mobo ASUS B250F Gaming|https://s.click.aliexpress.com/e/_DF8cacJ|
|CPU Intel i7 7700|https://s.click.aliexpress.com/e/_DllhiMf|
|HyperX Fury DDR4 2400MHz|https://s.click.aliexpress.com/e/_DmuaNi7|
|NVME Gen4 Kingston NV2|https://s.click.aliexpress.com/e/_DdL1G4J|
|Wireless & Bluetooth with AirDrop|https://s.click.aliexpress.com/e/_Dkbexrv| -->
