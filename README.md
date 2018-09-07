# Lenovo G50-80 | macOS Mojave

Hackintosh for Lenovo G50-80 

## Specs

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Intel i5-5200u (2.20Ghz up to 2.70Ghz)
Graphics | Intel Graphics HD 5500 (with Radeon R5 M330 [disabled])
RAM     | 4GB 1600Mhz DDR3 + 2GB 1600Mhz DDR3
Audio   | Conexant CX20752
Storage | 1TB HDD
Touchpad | ELAN Touchpad

## Features

* Supports 10.14
* CPU native support located in `/CLOVER/ACPI/patched`
* The sound card is CX20752, fake with `AppleALC`, layout-id: 3; and injection information is located at `/CLOVER/config.plist`
* Touchpad driver using `VoodooI2C`, support for multiple gestures; touchpad boot can be used normally, no drift, no wakeup
* Native Brightness hotkey support, related file is located at `/CLOVER/ACPI/patched/SSDT-LGPA.aml`
* Full support Intel HD Graphics with 2048MB (ig-plaform-id and kexts)

## Credits

- [RehabMan](https://github.com/RehabMan) Updated [OS-X-ACPI-Battery-Driver](https://github.com/RehabMan/OS-X-ACPI-Battery-Driver) and [OS-X-Clover-Laptop-Config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config) and [OS-X-FakeSMC-kozlek](https://github.com/RehabMan/OS-X-FakeSMC-kozlek) and [OS-X-Voodoo-PS2-Controller](https://github.com/RehabMan/OS-X-Voodoo-PS2-Controller) for maintenance

- [vit9696](https://github.com/vit9696) Updated [Lilu](https://github.com/acidanthera/Lilu) and [AppleALC](https://github.com/acidanthera/AppleALC) and [WhateverGreen](https://github.com/acidanthera/WhateverGreen) for maintenance

- [Piker-Alpha](https://github.com/Piker-Alpha) Updated [CPU Power Management](https://github.com/Piker-Alpha/ssdtPRGen.sh) for maintenance

- [alexandred](https://github.com/alexandred) and [hieplpvip](https://github.com/hieplpvip) Updated [VoodooI2C](https://github.com/alexandred/VoodooI2C) for maintenance

- [daliansky](https://github.com/daliansky) for [README Template](https://github.com/daliansky/XiaoMi-Pro/blob/master/README.md)

## Installation

To create a USB macOS Mojave installer be sure to carefully follow this tutorial [macOS Moajve Public Beta](https://www.tonymacx86.com/threads/how-to-create-a-macos-mojave-public-beta-installation-usb.254626/).

A complete EFI archive will be available at [releases](https://github.com/marcomarinho/Lenovo-G50-80/releases) page.

If the trackpad doesn't work during installation, please plug a wired mouse or a wireless mouse projector before the installation. After the installation completes, open `Terminal.app` and type `sudo kextcache -i /`. Wait for the process ending and restart the device. Enjoy your trackpad!


## Change Log:
