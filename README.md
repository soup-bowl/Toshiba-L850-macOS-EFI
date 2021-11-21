# 🍏 Toshiba Satelite Pro L850-1UJ, EFI Partition
Contains all the EFI data to start-up using Clover. **Secure boot must be disabled**. [Read more about this Hackintosh build here](https://www.soupbowl.io/2020/04/toshiba-satellite-pro-l850-hackintosh-revisited/).

This is the contents of the EFI folder, so ensure you clone this into the EFI partition's `EFI` folder.

## 🚀 Functionality
- ✅ Screen (full graphics)
- ✅ Display brightness (media keys don't work)
- ✅ Keyboard & trackpad
- ✅ Battery monitor
- ✅ USB
- ✅ Ethernet (registers as eth0 - App Store/FaceTime works)
- ✅ Speakers
- ❌ Suspend
- ❌ WiFi (Using Edimax N150 using [Chris111 drivers](https://github.com/chris1111/Wireless-USB-Adapter-Clover))
- ❌ Keyboard brightness controls

## 💻 Versions
### 🥾 Bootloader
Clover 5118. [Original configuration source](https://github.com/RehabMan/OS-X-Clover-Laptop-Config/blob/master/config_HD4000_1366x768.plist).

### 🧩 Kexts

Kext                 | Version     | Source
-------------------- | ----------- | ------
ACPI Battery Manager | 1.90.1      | https://github.com/RehabMan/OS-X-ACPI-Battery-Driver
Lilu                 | 1.4.9       | https://github.com/acidanthera/Lilu
Realtek RTL8111      | 2.3.0       | https://github.com/RehabMan/OS-X-Realtek-Network
Realtek WLAN U       | 1830.32.b17 | https://github.com/RehabMan/OS-X-Realtek-Network
Realtek WLAN U1827   | 1827.4.b36  | https://github.com/RehabMan/OS-X-Realtek-Network
VirtualSMC           | 1.1.8       | https://github.com/acidanthera/VirtualSMC
VoodooHDA            | 2.9.2       | https://sourceforge.net/projects/voodoohda
VoodooPS2Controller  | 1.9.2       | https://bitbucket.org/RehabMan/os-x-voodoo-ps2-controller

## ℹ️ Tips
### Mount EFI
Mount the EFI partition in macOS using:
```
sudo diskutil unmount disk0s1
```

Mount EFI in Linux LiveUSB:
```
sudo mount /dev/sda1 /mnt
```

### Clear NVRAM
When verbose is enabled, it can get 'stuck'. To disable it, clear the NVRAM. Press F11 then select reboot.
