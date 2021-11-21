# Toshiba Satelite Pro L850-1UJ, EFI Partition (Clover 5118)
Contains all the EFI data to start-up using Clover. **Secure boot must be disabled**.

WiFi chip doesn't work, so use a WiFi dongle (Edimax works fine). This isn't a pre-installed kext, use the installer packaged with this repo.

Mount the EFI partition in macOS using:
```
sudo diskutil unmount disk0s1
```

