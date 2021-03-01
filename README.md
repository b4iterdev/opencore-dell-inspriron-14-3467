# OpenCore EFI Bootloader for Dell Inspiron 14 3467
OpenCore EFI for Dell Inspriron 14 3467 (Intel Core i5-7200U - HD620)
| CPU | Intel Core I5 - 7200U |
|:---:| :-:                   |
| RAM | 4GB-DDR4              |
| GPU | Intel HD 620 ~ 1500MB Vram|
| Audio | Realtek ALC-256 (layout-id=11) |
# Notes:
OS Support: MacOS Mojave and newer (Catalina Working ). In the future I will continue maintaining this EFI.

At the moment I'm using HDD 5400rpm which is really slow, so until I have a new SSD I won't upgrade to BigSur.

Everything works except brightness hotkey (use Fn + S and Fn + B to change brightness ).

If you have problems with audio, use ALCPlugFix.  

This EFI is only for Dell Inspiron 14 - 3467, if you are using dell laptop with the same specs, to the following [this](https://dortania.github.io/OpenCore-Post-Install/usb/) guide to repatch USB Port.

* You might also want to patch Battery Indicator as this device doesn't need to patch.
