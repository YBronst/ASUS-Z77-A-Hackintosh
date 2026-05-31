# ASUS-Z77-A-Hackintosh

## EFI BUILD: ASUS Z77-A + Intel i7-3770K (Ivy Bridge)

- **Platform:** Ivy Bridge Desktop, OpenCore
- **Build Date:** March 20, 2026
- **Status:** Fully working configuration for macOS Catalina

**BOOTLOADER SPECIFICATIONS:**
- OpenCore v1.0.7 (Release March 20, 2026)
- Target SMBIOS: iMac13,2
- Video Kext: WhateverGreen v1.7.1 (Release Jul 7, 2025)
- NVRAM Boot-Args: keepsyms=1 debug=0x100 alcid=3 agdpmod=ignore -wegswitchgpu -cdfon -xcpm

**HARDWARE CONFIGURATION:**
- CPU: Intel Core i7-3770K (Ivy Bridge)
- RAM: 32 GB (4 x 8 GB) Samsung DDR3
- MB: ASUS Z77-A (Intel Z77 Express Chipset)
- Audio: Realtek ALC887 (Active layout-id: 3)
- iGPU: Intel HD Graphics 4000 (Set as empty framebuffer for hardware acceleration / headless mode)
- dGPU: AMD Radeon RX 580 (Native dGPU for display output)
- Storage: Samsung SSD 860 EVO 500GB (SATA interface, TRIM support active)

**macOS COMPATIBILITY:**
- Installed OS: macOS Catalina 10.15.7 (19H2) | Released: Sept 24, 2020
- Native Support: Up to macOS Big Sur 11.7.10 (20G1427) | Released: Sept 11, 2023
- Patch Support via OCLP: macOS 13 Ventura / macOS 14 Sonoma / macOS 15 Sequoia

**IMPORTANT BOOT NOTES:**
- Generate new serial numbers in PlatformInfo -> Generic before using this EFI.
- Required BIOS Settings: VT-d (Disabled), CSM (Disabled), Fast Boot (Disabled), OS Type (Other OS / Windows 8 UEFI).
- AMD RX 580 and Intel HD 4000 work natively in Big Sur. No post-install root patches required.
