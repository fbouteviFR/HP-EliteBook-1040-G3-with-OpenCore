# HP-EliteBook-1040-G3-with-OpenCore

HP EliteBook 1040 G3 with OpenCore

Here attached the content of the EFI partition

### Status: Running

Currently running:

| Component     | Version      |
| ------------- | ------------ |
| macOS version | 11.3.1 (20E241 |
| OpenCore      | 0.6.9        |
| BIOS version  | TBC        |

## Hardware info

| Component | Model                                   |
| --------- | --------------------------------------- |
| CPU       | Intel(R) Core(TM) i5-6300U    |
| Memory    | 8GB                       |
| Storage   | KXG50ZNV1T02 TOSHIBA                 |
| Display   | 14" 1920x1080                 |
| GPU       | Intel HD Graphics 520                          |
| WLAN      | Intel 8260 |

## Status

### Working

- [x] Keyboard (including all media keys)
- [x] Battery indicator (number of cycles reported)
- [x] Display brightness (keys F5 and F6)
- [x] Audio
- [x] Ethernet
- [x] iCloud services - iMessage, FaceTime, AppStore
- [x] Camera
- [x] Microphone
- [x] Bluetooth
- [x] Sleep/wake (You can configure wake on open lid if you want)
- [x] Trackpad as a mouse
- [x] HDMI video

## Compatible BIOS settings

| Parameter     | Value      |
| ------------- | ------------ |
| TPM Device | Hidden |
| TPM State | Disable |
| TPM Activation Policy | No prompts |
| Fast Boot | Disable |
| Network (PXE) Boot | Disable |
| Configure Legacy Support and Secure Boot | Legacy Support Disable and Secure Boot Disable |
| HP Application Driver | Disable |
| Wake On LAN | Disabled |
| Extended Idle Power States | Enable |
| Wake when Lid is Opened | Enable |
| Fingerprint Device | Disable |
| Video Memory Size | 64 MB |
| Intel Software Guard Extensions (SGX) | Disable |
| Virtualization Technology (VTx) | Disable |
| Virtualization Technology for Directed I/O (VTd) | Disable |
| Deep Sleep | On |
| Media Card Reader | Disable | 
| Trusted Execution Technology (TXT) | Disable | 
  
## Post-install

sudo pmset autopoweroff 0
sudo pmset powernap 0
sudo pmset standby 0
sudo pmset proximitywake 0
sudo pmset tcpkeepalive 0

Enjoy it :)

## CREDITS

- [Acidanthera](https://github.com/acidanthera)
- [Dortania OC guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [Rehabman's battery patch guide](https://www.tonymacx86.com/threads/guide-how-to-patch-dsdt-for-working-battery-status.116102/) and [Rehabman's ACPI hotpatching guide](https://www.tonymacx86.com/threads/guide-using-clover-to-hotpatch-acpi.200137/)
- [OpenWireless and itlwm](https://github.com/OpenIntelWireless/itlwm)
- Thanks also to Hackintool / great tool
- Thanks also to OpenCore Configurator / great tool too :)
