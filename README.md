# Dell-Optiplex-3040-SFF-Hackintosh-Big-sur-11.2.3-Guide
This is a list of files and settings to get your Dell Optiplex 3040 SFF setup and running with Big Sur!


This guide assumes that you are following the Dortania Guide (https://dortania.github.io/getting-started/) to get your hackintosh going. This guide uses OpenCore and NOT Clover


Bios Settings: Set BIOS DEFAULTS and ensure that UEFI boot and AHCI are enabled.

Specs:
Intel Core i5 6500 (SKYLAKE)
8GB DDR3L (this PC only takes DDR3L) 
iGPU (Intel HD Graphics 530)

Optional (for Wifi and Bluetooth
YOUBO PC Hackintosh Dual Band WiFi Card BCM94360CD 
https://www.amazon.com/gp/product/B082X8MBMD/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1

This Wifi card works 100% with no additional kexts, but does not come with a half height bracket. I had to Cut the bracket on both ends for it to fit. The board also does not have a required USB header (the header on the board is a proprietary Dell connector) and had to solder the included 4 pin usb header into a regular USB cable and run it through the back.

Working:
Everything but sleep (seems to be an iGPU problem)




