# Toshiba Satelite Pro L850-1UJ, EFI Partition (Clover 5118)
Contains all the EFI data to start-up using Clover. **Secure boot must be disabled**.

WiFi chip doesn't work, so use a WiFi dongle (Edimax works fine). This isn't a pre-installed kext, use the installer packaged with this repo.

Mount the EFI partition in macOS using:
```
sudo diskutil unmount disk0s1
```

## Versions
### Bootloader
Clover 5118.

### Kexts

Kext                 | Version     | Source
-------------------- | ----------- | ------
ACPI Battery Manager | 1.90.1      |
Lilu                 | 1.4.9       |
Realtek RTL8111      | 2.3.0       |
Realtek WLAN U       | 1830.32.b17 |
Realtek WLAN U1827   | 1827.4.b36  |
VirtualSMC           | 1.1.8       |
VoodooHDA            | 2.9.2       |
VoodooPS2Controller  | 1.9.2       |
