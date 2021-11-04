# HACKINTOSH-ASUS-X441UV
**Laptop specification:**
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

**Working**
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
- AirDrop and Handoff (I think it works, I don't have another Apple device to test it)
- Etc

**Not Working**
- GeForce 920mx (Not supported by Monterey)
- Sleep (sleep on my laptop is broken, both on Windows or macOS)

