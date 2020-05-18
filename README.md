# Acer Aspire VX15 Hackintosh

I recommend using OpenCore it's better and smoother. If you want to use OpenCore see here:  
https://github.com/dongcodebmt/VX5-591G-OpenCore
 
__My Specs__

| Specs | Details |
|------------|-------------------------------|
| Model | Acer Aspire VX15 (VX5-591G) |
| OS | macOS Catalina 10.15.4 |
| CPU | Intel(R) Core(TM) i5 7300HQ |
| RAM | 16 GB DDR4 2400MHz |
| iGPU | Intel HD Graphics 630 |
| dGPU | NVIDIA GeForce GTX 1050M |
| Touchpad | ELAN 0501 |
| Wireless | Intel® Dual Band Wireless-AC 7265 |
| Audio | ALC255 |

![Specs](/image.png)

__Tested and working__

- [x] Intel HD Graphics 630
- [x] USB
- [x] Webcam
- [x] HDMI + HDMI Audio
- [x] LAN
- [x] Screen brightness
- [x] Battery status
- [x] Sleep/Wake
- [x] Audio + Headphone + Internal Mic
- [x] TouchPad with gestures
- [x] Keyboard with backlight (Some function keys not work)
- [x] Bluetooth (Can't off) 

__Not tested__

- [ ] USB C (I don't have a device to test)

__Not working__

- [ ] NVIDIA GeForce GTX 1050M
- [ ] SD Card reader
- [ ] WiFi
- [ ] and a few other minor bugs

For wifi and bluetooth to work you need to replace another wireless card

## Guide

__BIOS Settings (Version 1.08)__

- Set Supervisor Password
- Disable Password on Boot
- Disable Secure Boot
- Set touchpad: Advance

__Clover config__

Use rehabman's config: `config_HD615_620_630_640_650.plist`   
I used SSDT files and patches from: https://github.com/dongcodebmt/VX5-591G-OpenCore   
Boot args: `alcid=30 keepsyms=1 debug=0x100`

__Fix Timezone (Dual Boot)__

See: https://www.tonymacx86.com/threads/fix-incorrect-time-in-windows-osx-dual-boot.133719/

## Credits

Thanks to RehabMan, Acidanthera, alexandred

*__Enjoy__*