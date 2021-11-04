# HACKINTOSH-ASUS-X441UV
## Laptop specification:
- CPU: Intel i3-6100U 2.30 GHz
- RAM: 2x4 GB
- iGPU: Intel HD 520
- dGPU: GeForce 920mx (disabled)
- WiFi: Broadcomm BCM94360HMB plus Bluetooth
- Ethernet: Realtek RTL8139/810x Fast Ethernet Adapter
- Audio Codec: Realtek ALC255
- Trackpad: I2C HID Device
- Keyboard: PS/2 Interface
- Storage: SSD TeamGroup CX2 Series 256 GB + HDD HGST 1 TB (both are SATA device)
- Monitor: Built-in monitor 14" HD resolution (1366x768)
- Boot Mode : UEFI
- Bootloader : OpenCore 0.7.5 release
- OS Version : macOS Monterey 12.0.1 Build 21A559

## Working
- QE/CI Graphics of iGPU HD 520
- Restart and Shutdown
- Internal Speaker, Headphone audio and Internal Mic
- Battery Indicator
- Brightness
- Brightness Button Up / Down
- Ethernet
- Wifi
- Bluetooth (detected as THIRD PARTY DONGLE, Monterey bug)
- Touchpad
- All USB Ports
- HDMI
- HDMI Audio
- AirDrop and Handoff (I think it works, I don't have another Apple device to test it)
- Etc

## Not Working
- GeForce 920mx (Not supported by Monterey)
- Sleep (sleep on my laptop is broken, both on Windows or macOS)

## **About Files**
- This EFI file is based from OpenCore bootloader, not working on Clover etc. 
- config.plist file is configured depended my device, please check again for any difference kext and other files depend your device.
- config.plist need to configure SMBIOS. 
- any errors and configuration changes are not my responsibility. please check your configuration again.

# *For updated kexts and other files, please check the main sources*
1. [Lilu](https://github.com/acidanthera/Lilu/releases) A kext to patch many processes, required for AppleALC, WhateverGreen, VirtualSMC and many other kexts. Without Lilu, they will not work.
2. [VirtualSMC](https://github.com/acidanthera/VirtualSMC/releases) Emulates the SMC chip found on real macs, without this macOS will not boot
3. [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases) Used for graphics patching, DRM fixes, board ID checks, framebuffer fixes, etc; all GPUs benefit from this kext.
4. [AppleALC](https://github.com/acidanthera/AppleALC/releases) Used for AppleHDA patching, allowing support for the majority of on-board sound controllers.
5. etc

Full list of files, please refer to [OpenCore tutorial](https://dortania.github.io/OpenCore-Install-Guide/).
