# OpenCore EFI Bootloader for Dell Inspiron 14 3467
OpenCore EFI for Dell Inspriron 14 3467 (Intel Core i5-7200U - HD620)
| CPU | Intel Core I5 - 7200U |
|:---:| :-:                   |
| RAM | 4GB-DDR4              |
| GPU | Intel HD 620 ~ 1500MB Vram|
| Audio | Realtek ALC-256 (layout-id=21) |
| Version | Opencore 0.6.9 |

![Screen Shot 2021-03-09 at 1 06 15 PM](https://user-images.githubusercontent.com/57698887/110426230-50186780-80d8-11eb-91bb-45d2d78e5b6e.png)

# Notes:
OS Support: MacOS HighSierra and newer (Upto BigSur!). In the future I will continue maintaining this EFI.

Before using this efi, go [here](https://github.com/OpenIntelWireless/itlwm/releases/) and download appropriate AirportItlwm.kext with your macOS version to /OC/Kexts (you don't need to re-snapshot the config as AirportItlwm are included).

At the moment I'm using HDD 5400rpm which is really slow, so until I have a new SSD I won't upgrade to BigSur.

Everything works except brightness hotkey (use Fn + S and Fn + B to change brightness, in VoodooPS2Controller brightness keys are f13 and f14).

~~If you have problems with audio, use ALCPlugFix. Instead use ComboJack~~.Audio works with layout-id 21 without any workaround

This EFI is only for Dell Inspiron 14 - 3467, if you are using dell laptop with the same specs, to the following [this](https://dortania.github.io/OpenCore-Post-Install/usb/) guide to repatch USB Port.

* You might also want to patch Battery [here](https://dortania.github.io/OpenCore-Post-Install/laptop-specific/battery.html#dsdt-patching) as this device doesn't need to patch.

# For HighSierra user:

For Opencore 0.6.9, macOS might not boot if you have AppleSecureBoot enabled with default value as HighSierra is now old, so you might want to disable by going to Mics -> SecureBootModel -> Disabled
