# Dell-Optiplex-3040-SFF-Hackintosh-Big-Sur-11.2.3-Guide
This is a list of files and settings to get your Dell Optiplex 3040 SFF setup and running with Big Sur!


This guide assumes that you are following the Dortania Guide (https://dortania.github.io/getting-started/) to get your hackintosh going. This guide uses OpenCore and NOT Clover


Bios Settings: Set BIOS DEFAULTS and ensure that UEFI boot and AHCI are enabled. DISABLE THE SERIAL PORT (Causes a black screen issue after boot with 
RX560)

BIOS Revision : 1.14.2

OpenCore Version : 0.6.7

Specs:

Intel Core i5 6500 (SKYLAKE)

8GB DDR3L (this PC only takes DDR3L) 

iGPU (Intel HD Graphics 530)
dGPU AMD RX 560 LP / Radeon Pro WX4100




*Optional (for Wifi, Bluetooth and Continuity Features)
YOUBO PC Hackintosh Dual Band WiFi Card BCM94360CD 
https://www.amazon.com/gp/product/B082X8MBMD/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1

This Wifi card works 100% with no additional kexts, but does not come with a half height bracket. I had to Cut the bracket on both ends for it to fit. The board also does not have a required USB header (the header on the board is a proprietary Dell connector) and had to solder the included 4 pin usb header into a regular USB cable and run it through the back.

Working:
Everything (with dGPU)

Not Working 
Sleep (With iGPU)



Make sure to input your Mac Address, Serial, Board Serial and UUID into the config! I have anonymized it. 
If you want to use your iGPU, you have to set your DeviceProperties > Add section to enable the iGPU. The settings in the guide under skylake work perfectly. 
If you are using a USB Bluetooth adapter, the Top Left - Rear USB port is set to internal in the usb map, if you wish for sleep to work properly, use this USB port, or change your USB map to match the port you wish to use.




