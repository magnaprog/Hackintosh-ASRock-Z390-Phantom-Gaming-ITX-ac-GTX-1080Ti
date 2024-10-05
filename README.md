# Hackintosh - ASROCK Z390 Phantom Gaming-ITX/ac

This repository contains the OpenCore configuration and necessary files to run macOS High Sierra 10.13.6 on ASROCK Z390 Phantom Gaming-ITX/ac with i9-9900K and GTX 1080 Ti.

## Hardware Specifications

- Motherboard: ASROCK Z390 Phantom Gaming-ITX/ac
- CPU: Intel Core i9-9900K
- GPU: NVIDIA GeForce GTX 1080 Ti
- RAM: [Your RAM specifications]
- Storage: [Your storage specifications]
- WiFi/Bluetooth: [Your WiFi/Bluetooth card model]

## Software Versions

- macOS: High Sierra 10.13.6 (17G66)
- OpenCore: 1.0.1 (Consider updating to latest version)

## What Works

- [x] NVIDIA GTX 1080 Ti (with Web Drivers)
- [x] Intel UHD 630 Graphics
- [x] Audio
- [x] Ethernet
- [x] USB Ports
- [x] Sleep/Wake
- [x] Power Management

## What Doesn't Work

- [ ] [List any non-working features]

## Installation

1. Create a bootable USB installer for macOS High Sierra
2. Clone this repository and copy the EFI folder to your USB drive's EFI partition
3. Boot from the USB drive and install macOS
4. After installation, copy the EFI folder to your system drive's EFI partition

## Post-Installation

1. Install NVIDIA Web Drivers for your specific macOS version
2. [Any other post-installation steps specific to your build]

## BIOS Settings

- Disable:
  - Secure Boot
  - CSM (Compatibility Support Module)
- Enable:
  - EHCI/XHCI Hand-off
  - Above 4G decoding
- Set SATA Mode to AHCI

## Notes

- This build is specifically for macOS High Sierra 10.13.6 due to NVIDIA GTX 1080 Ti compatibility
- Ensure you're using the correct SMBIOS for your configuration (iMac19,1 recommended for this build)
- Always backup your data before making changes to your system

## Troubleshooting

If you encounter issues:
1. Enable verbose boot by adding `-v` to your boot-args
2. Check your config.plist for any misconfigurations
3. Ensure all kexts and drivers are up to date
4. Refer to [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) for detailed troubleshooting

## Credits

- [Acidanthera](https://github.com/acidanthera) for OpenCore and many kexts
- [Dortania](https://github.com/dortania) for their detailed OpenCore guides
- [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [NVIDIA Web Drivers](https://www.nvidia.com/download/driverResults.aspx/162105/en-us)

## Disclaimer

This project is for personal use and educational purposes only. Use at your own risk. I am not responsible for any damage to your hardware or any loss of data.