<h1 align="center"> macOS on HP ProBook 440 G7 </h1>

<p align="center">
  <img src="https://github.com/yusufklncc/HP-ProBook-440-G7-Hackintosh/blob/main/Resources/hp-probook-440-g7.png" alt="ProBook 440 G7" width="750">
</p>

<h4 align="center"> OpenCore config for Hackintosh Lenovo Thinkpad E570 </h4>

<p align="center">
<a href="https://www.apple.com/macos/sonoma-preview/">
  <img src="https://img.shields.io/badge/macOS-Sonoma-green" width="170"/> </a>
<a href="https://github.com/acidanthera/OpenCorePkg/releases">
  <img src="https://img.shields.io/badge/OpenCore-0.9.8-9cf" width="160"/> </a>
<a href="https://github.com/yusufklncc/HP-ProBook-440-G7-Hackintosh/releases">
  <img src="https://img.shields.io/badge/release-EFI-blue.svg" width="120"/> </a>
  <a href="https://github.com/yusufklncc/HP-ProBook-440-G7-Hackintosh/issues"> 
  <img src="https://img.shields.io/github/issues/yusufklncc/HP-ProBook-440-G7-Hackintosh" width="145"/> </a>
</p>
<p align="center">
<a href="https://t.me/yusufklncc">
  <img src="https://img.shields.io/badge/-@yusufklncc-2CA5E0?logo=Telegram&logoColor=white" width="150"/> </a>
<a href="https://www.youtube.com/c/yusufklncc">
  <img src="https://img.shields.io/badge/-@yusufklncc-red?logo=YouTube&logoColor=white" width="150"/> </a>
<a href="https://www.paypal.com/paypalme/sevenpay">
  <img src="https://img.shields.io/badge/-@sevenpay-white?logo=PayPal" width="140"/> </a>
<a href="https://www.buymeacoffee.com/yusufklncc">
  <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" width="150"/> </a>

## Table of Contents
  - [Screenshots](#screenshots-)
  - [Original Hardware](#original-hardware--)
  - [macOS Update History](#macos-update-history)
  - [What's working](#whats-working--)
  - [What's not working](#whats-not-working--)
  - [Installation Steps](#installation-steps)
  - [Credits](#credits)
  - [Donate](#-donate---ba%C4%9F%C4%B1%C5%9F-)
  
## Screenshots 📷

### Sonoma
<p align="center">
  <img src="https://github.com/yusufklncc/HP-ProBook-440-G7-Hackintosh/blob/main/Resources/macOS%20Desktop/macos-sonoma.png">
</p>

## Original Hardware  💻
Type | Spec | Status
:---------|:---------|:----------
Model      | HP ProBook 440 G7 | ✅
Variant      | 869D | ✅
BIOS      | S71 Ver. 01.19.00 08/02/2020 | ✅
CPU              | Intel(R) Core(TM) i7-10510U CPU @ 1.80GHz Comet Lake | ✅
RAM           | 8 GB DDR4 | ✅
Internal Graphics Card | Intel(R) CometLake-U GT2 (UHD Graphics 620) | ✅
Wi-Fi             | Intel AX201 Wi-Fi 6 (802.11ax) | ✅
Ethernet          | Realtek RTL8111/8168/8411 | ✅
SSD         | WDC PC SN730 SDBPNTY-256G-1101 | ✅
Audio       | Realtek ALC 236 | ✅
Touchpad | SYNA30A5:00 06CB:CDEB | ✅
Fingerprint |  | ❌
Camera | HP HD - IR Camera | ❌
  

## macOS Update History
- ✅ macOS Sonoma 14.3


## What's working  💻
Type | Status
:---------|:---------
Turbo boost and CPU frequency stage |  ✅
Intel UHD Graphics 620              |  ✅
Brightness control                  |  ✅
HDMI                                |  ✅
Audio Realtek ALC 236               |  ✅
Realtek Ethernet RTL8111            |  ✅
Intel AX201 Wi-Fi and Bluetooth     |  ✅
USB 3.0 and Type-C (with Port Map)  |  ✅
Touchpad (14 gestures are working)  |  ✅
Battery status                      |  ✅
S3 Sleep / Wake   |  ✅
S4 Hibernation / Wake   |  ✅
Shutdown / Reboot   |  ✅
Fn shortcut keys   |  ✅

## What's not working  💻
Type | Status
:---------|:---------
Touchpad Clicking | ❌
Camera   |  ❌

## boot-args Used
boot-arg | Info
:---------|:---------
-v | Enables verbose.
swd_panic=1 | Avoids issue where going to sleep results in a reboot
-noDC9 | Fixes sleep issues.

## Installation Steps

### Downloading OSX Image
- Click to Google Drive or Ya.Disk link and download it.
  - [Sonoma](https://github.com/yusufklncc/Hackintosh-for-All-Computers#-macos-ventura-)
  - [Ventura](https://github.com/yusufklncc/Hackintosh-for-All-Computers#-macos-ventura-)
  - [Monterey](https://github.com/yusufklncc/Hackintosh-for-All-Computers#macos-monterey)
  - [Big Sur](https://github.com/yusufklncc/Hackintosh-for-All-Computers#macos-big-sur)
  
### Writing OSX Image
- Unzip the zip file to desktop.
- Download [balenaEtcher](https://www.balena.io/etcher/).
- Open program and click to `Flash from file`.
- Select the OSX image `.raw` file from the popup window.
- Click to `Select target` and select OSX image.
- Click to `Flash!` and allow app in popup window.
<p align="center">
  <img src="https://user-images.githubusercontent.com/78423442/154849816-0a04602a-9064-4780-9d4e-ed86254b4fea.png">

- When writing is finished, `remove` the USB stick and plug it back in.

### Setting EFI Folder
- When you plug USB back, you can see EFI partition in "My Computer"
- Open EFI partition.
- Delete default files.
- Copy downloaded EFI folder to EFI partititon.
- Now you can boot from USB.

### Setting BIOS Settings 
  - Before you start, reset your BIOS settings to default.
  - `Disable`
    - Secure Boot

    
### macOS Installation
- Now let's turn off our computer and boot from USB. Choose the `Install macOS Sonoma` (whatever you have) option on OpenCore menu and go to the installation screen.
- <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%201.png">
- What to do on the following screens:
  - Select language and continue.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%202.png">
  - Open `Disk Utility` from the menu to prepare our disk.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%203.png">
  - Select `Show All Devices` from the `View` option and select the name of our disk and click `Erase`.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%204.png">
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%205.png">
  - Rename the disk and erase as `APFS/GUID`.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%206.png">
  - Now close `Disk Utility` and select `Install macOS Sonoma` then next next next.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%208.png">
  - Select renamed disk and click continue.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%2010.png">
  - When the installation is finished,  `macOS Installer` option will be selected automatically every boot step until this option is `gone`.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%2011.png">
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%2012.png">
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%2013.png">
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%2014.png">
  - After last boot, the language selection screen will welcome us. Select language and continue.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%2015.png">
  - Don't login `iCloud` account and continue. Because we need to set our `serial numbers and ROM for iCloud and iMessage`.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%2016.png">
  - Now we can see `Desktop`.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/Installation/macOS%2017.png">

### Post Installation

- Open config file with `Text Edit`.
  - Search `HideAuxiliary` and change `false` value to `true`.
  - Search `SecureBootModel` and change `Disabled` value to `Default`.
  - Search `boot-args` and delete `-v` argument.
- Now we have to set our serial numbers and ROM value.
  - Download [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS/archive/refs/heads/master.zip) and open .command file. If program asks `Download Python` download it. After that select option 3.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/GenSMBIOS/GenSMBIOS%201.png">
  - Now list 5 SMBIOS first. `MacBookPro15,4`
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/GenSMBIOS/GenSMBIOS%202.png">
  - Select and copy first Serial.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/GenSMBIOS/GenSMBIOS%203.png">
  - Go [check](https://checkcoverage.apple.com/) serial number. Your serial should be like this. If not, try second serial.
  - <img src="https://github.com/yusufklncc/Lenovo-Thinkpad-E570-Hackintosh/blob/main/Resources/GenSMBIOS/Check%20Serial.png">
  - Search MacBookPro15,1 and replace `Type > SystemProductName, Serial > SystemSerialNumber, Board Serial > MLB and SmUUID > SystemUUID` values. Now we will set our ROM value.
  - Go `System Setting > Netwotk > Ethernet > Details > Hardware`. If our MAC adress is `54:1A:AF:43:70:CA` remove `:` characters = `541AAF4370CA`. Convert it to [Base64](https://base64.guru/converter/encode/hex). 
  - Now we have `VBqvQ3DK`. Replace this with ROM value and save config file.
  - Restart computer and press `Space` key on OpenCore menu. Then enter `ResetNVRAM`. After that BIOS settings may change. Check it and boot macOS.
  - Now you can login iCloud, iMessage or other apple services and you can use macOS.
      
## Credits
  
 - [Dortania](https://dortania.github.io) for developing OpenCore.
 - [Apple](https://www.apple.com) for macOS.
 - [Acidanthera](https://github.com/acidanthera) for most of the kexts.
 - [RehabMan](https://github.com/RehabMan) for battery patches.
 - [Sniki](https://github.com/Sniki) for USB kext.
 - And anyone else that helped to develop and improve hackintoshing.

<h1 align="center"> Donate - Bağış </h1>
<p align="center">
<a href="https://github.com/yusufklncc/yusfklncc/blob/main/Donate%20-%20Ba%C4%9F%C4%B1%C5%9F.md">
  <img src="https://github.com/yusufklncc/yusfklncc/blob/main/Resources/Donate.png" width="300">
