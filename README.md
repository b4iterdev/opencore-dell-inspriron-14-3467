# OpenCore EFI Bootloader for Dell Inspiron 14 3467
OpenCore EFI for Dell Inspriron 14 3467 (Intel Core i5-7200U - HD620)
| CPU | Intel Core I5 - 7200U |
|:---:| :-:                   |
| RAM | 8GB-DDR4              |
| GPU | Intel HD 620 ~ 1500MB Vram|
| Audio | Realtek ALC-256 (layout-id=21/alcid=21) |
| Version | Opencore 1.0.5 |

![image](https://user-images.githubusercontent.com/57698887/119744931-47edee00-beb7-11eb-9d00-054610c87f8a.png)

# Notes:
OS Support: MacOS HighSierra and newer (Upto Ventura 13.7.10!). In the future I will continue maintaining this EFI.

Before using this efi, go [here](https://github.com/OpenIntelWireless/itlwm/releases/) and download appropriate AirportItlwm.kext with your macOS version to /OC/Kexts (you don't need to re-snapshot the config as AirportItlwm are included in config.plist).

Everything works except brightness hotkey (use Fn + S and Fn + B to change brightness, in VoodooPS2Controller brightness keys are f13 and f14).

~~If you have problems with audio, use ALCPlugFix. Instead use ComboJack~~.Audio works with layout-id 21 without any workaround. Other option is update alcid=21 (NVRAM->Add).

This EFI is only for Dell Inspiron 14 - 3467, if you are using dell laptop with the same specs, to the following [this](https://dortania.github.io/OpenCore-Post-Install/usb/) guide to repatch USB Port.

* You might also want to patch Battery [here](https://dortania.github.io/OpenCore-Post-Install/laptop-specific/battery.html#dsdt-patching) as this device doesn't need to patch.

# For HighSierra user:

For Opencore 0.6.9, macOS might not boot if you have AppleSecureBoot enabled with default value as HighSierra is now old, so you might want to disable by going to Mics -> SecureBootModel -> Disabled
