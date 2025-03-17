# SteamFork&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Latest Version](https://img.shields.io/github/v/release/SteamFork/distribution.svg?color=1384B5&label=latest%20version&style=flat-square)](https://github.com/SteamFork/distribution/releases/latest) [![Activity](https://img.shields.io/github/commit-activity/m/SteamFork/distribution?color=1384B5&style=flat-square)](https://github.com/SteamFork/distribution/commits) [![Discord](https://img.shields.io/discord/1245092101193072650?color=1384B5&label=chat&style=flat-square)](https://discord.gg/AQ5rtQstCf)

SteamFork is a SteamOS-based operating system with improved hardware compatibility.  It is designed to provide the same experience as SteamOS on a SteamDeck.

## Features
* Works on a variety of devices from ASUS, Antec, Atari, Ayaneo, Ayn, and GPD along with MiniPCs and other computers with compatible hardware.
* Provides a full SteamOS UI/UX experience, including SteamOS's desktop mode.
* SteamFork is an atomic distribution with simple rollback and recovery options.
* SteamOS is our upstream, making SteamFork the only active Linux gaming solution truly derived from SteamOS.
* Minimal changes are made to SteamOS to preserve compatibility with Steam Deck plugins, software, and documentation.
* RGB is off by default on supported devices, RGB will flash on low battery when available.
* Offers improved fan curves on supported devices from Ayaneo and Ayn.
* Includes power management optimizations ported from [JustEnoughLinuxOS](https://github.com/JustEnoughLinuxOS).
* Supports booting from removable media such as usb drives and micro sd cards (64GB minimum) and dual boot with Windows.
* Compatible with Epic Games Store, GoG, and Amazon Prime Gaming via Heroic which is available for installation in discover.

Review the device support [table](https://github.com/SteamFork#device-support) below along with our [Wiki](https://wiki.steamfork.org) for more information about our project.

## Screenshots
### Ayn Loki Max
<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/SteamFork/.github/main/profile/.images/20240609-max-1.jpg"/></td>
    <td><img src="https://raw.githubusercontent.com/SteamFork/.github/main/profile/.images/20240609-max-2.jpg"/></td>
  </tr>
</table>

### Ayaneo 2S
<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/SteamFork/.github/main/profile/.images/20240525-2s-1.jpg"/></td>
    <td><img src="https://raw.githubusercontent.com/SteamFork/.github/main/profile/.images/20240525-2s-2.jpg"/></td>
  </tr>
</table>

### Ayaneo Flip KB
<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/SteamFork/.github/main/profile/.images/20240525-flip-1.jpg"/></td>
    <td><img src="https://raw.githubusercontent.com/SteamFork/.github/main/profile/.images/20240525-flip-2.jpg"/></td>
  </tr>
</table>

## Licenses
SteamFork is a Linux distribution that is made up of many open-source components, and each component is provided under its respective license.  Unless otherwise noted, the content of this project itself is made available under the terms of the MIT license.  See [LICENSE](https://github.com/SteamFork/distribution/blob/main/rootfs/steamfork/LICENSE) for details.

## Community
We use Discord for project related discussion.  Everyone is welcome to join our community by clicking the invitation link below.
* [SteamFork Discord](https://discord.gg/AQ5rtQstCf)

## Device Support
SteamFork is supported on sponsored devices listed below however it also works great on modern laptops, desktops, and mini PCs with Intel and AMD processors and graphics.  Devices without sponsors are not actively tested by a dedicated maintainer and may have unknown issues.
| Manufacturer | Product | Sponsor <sup>1</sup> |
| -- | -- | -- |
| Anbernic | [Win600](https://wiki.steamfork.org/devices/anbernic/win600) | Community Verified |
| ANTEC | [Core HS](antec/core-hs.md) <sup>2</sup> | Community Verified |
| ASUS | [ROG Ally / Ally X](https://wiki.steamfork.org/devices/asus/rog-ally) | [flukejones](https://github.com/flukejones) |
| Atari | [VCS](atari/vcs.md) | Community Verified |
| AYANEO | [2](ayaneo/ayaneo-2) | Community Verified |
| AYANEO | [2S](https://wiki.steamfork.org/devices/ayaneo/ayaneo-2s) <sup>3</sup> | [Fewtarius](https://github.com/fewtarius) |
| AYANEO | [Air / Air Pro](ayaneo/air.md) | Community Verified |
| AYANEO | [Air 1S](https://wiki.steamfork.org/devices/ayaneo/air-1s) <sup>3</sup> | [winghugs](https://github.com/winghugs) |
| AYANEO | [Air Plus (AMD 6800U)](https://wiki.steamfork.org/devices/ayaneo/air-plus-6800u) | [uejji](https://github.com/uejji) |
| AYANEO | [Flip DS](https://wiki.steamfork.org/devices/ayaneo/flip-ds) <sup>2,4</sup> | [uejji](https://github.com/uejji) |
| AYANEO | [Flip KB](https://wiki.steamfork.org/devices/ayaneo/flip-kb) <sup>2</sup> | Community Verified by [Fewtarius](https://github.com/fewtarius) |
| AYANEO | Geek | Community Verified by [alexapple79](https://www.youtube.com/watch?v=4iBE-PUC_0Y) |
| AYANEO | Next, Next Lite, Next Pro | Community Verified |
| AYANEO | [Slide](ayaneo/slide.md) <sup>2</sup> | Community Verified |
| Ayn | [Loki Max](https://wiki.steamfork.org/devices/ayn/loki-max) | [Fewtarius](https://github.com/fewtarius) |
| Ayn | [Loki Zero](ayn/loki-zero) | Community Verified |
| GPD | Win 2 | Community Verified by [PacoA](https://github.com/pacoa-kdbg) |
| GPD | [Win 4 (AMD 6800U)](https://wiki.steamfork.org/devices/gpd/win4-6800u) | [anthonycaccese](https://github.com/anthonycaccese) |
| GPD | Win 4 (AMD 7840U) | Community Verified by [Maeiourk](https://github.com/maeiourk) |
| GPD | Win Mini | Community Verified |
| MSI | [Claw A1M](https://wiki.steamfork.org/devices/msi/claw-a1m) | Community Verified |
| ONEXPLAYER | Mini (Intel 1195G7) | Community Verified by Joex |
| ONEXPLAYER | OneXFly F1 Pro (AMD HX 370) | Community Verified by [Reiyume](https://github.com/reiyume) |

> [!NOTE]
> 1. Sponsored devices are fully supported by its maintainer.  Support for unsponsored and community verified devices may vary.<br>
> 2. Some AMD 7000 series devices do not support S3 sleep and must be configured for Modern Standby + s0i3.  This setting is locked down on many Ayaneo devices and must be enabled using a third party helper.  Follow the [process on the Wiki](https://wiki.steamfork.org/troubleshooting/#enabling-modern-sleep-on-7000-series-amd-based-devices) to configure your device.
> 3. Requires a BIOS update for modern sleep to work correctly.
> 4. Support for these devices is still a work in progress.  Expect bugs or incomplete/missing features as support is being added.  Refer to the [specific device's page on the Wiki](https://wiki.steamfork.org/devices/) for more information.

### Documentation
SteamFork documentation is hosted on our [Wiki](https://wiki.steamfork.org).  There you will find answers to [Frequently Asked Questions](https://wiki.steamfork.org/faqs/), [Build](https://wiki.steamfork.org/contribute/build/) and [Device Quirk](https://wiki.steamfork.org/contribute/quirks/) development instructions, and much more.

### Sponsorship
Sponsoring a device is a commitment to maintaining support for your device by validating, testing, and bugfixing any issues that may arise.  Adding support for a device's basic features is straight forward, however, it can become far more technical to add support for features such as fan control.  If you are interested in sponsoring your device, follow the process below.

1. Create a GitHub account if you do not already have one.
2. Boot the SteamFork installation image.
3. Create a device quirk using the [quirk creation tool](https://wiki.steamfork.org/contribute/quirks/) included with the distribution.  Minimum requirements are gamescope resolution, and rotation if needed.
4. Create a pull request to the [SteamFork Device Support](https://github.com/SteamFork/distribution/tree/main/PKGBUILD/steamfork-device-support) package with your new addition.
5. Open and take ownership of any issues specific to your device on [discord](https://github.com/SteamFork#community).
6. When ready to begin sunsetting support for your device, generate and PR new quirk with the `--supported false` property.

## Downloads 
Downloads are hosted at [SteamFork.org](https://www.steamfork.org/images/installer/) and updates are available OTA.  A download link to the latest installation ISO can be
 found below.

| Branch | URL | Checksum | Version |
| -- | -- | -- | -- |
| Primary | [LATEST](https://www.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso) | [SHA256](https://www.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso.sha256) | [![Version](https://img.shields.io/github/release/SteamFork/distribution.svg?color=156C9C&label=&style=flat-square)](https://github.com/SteamFork/distribution/releases/latest) |
| New York | [LATEST](https://www1.ny.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso) | [SHA256](https://www1.ny.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso.sha256) |||
| Dallas | [LATEST](https://www1.da.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso) | [SHA256](https://www1.da.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso.sha256) |||
| San Jose | [LATEST](https://www1.sj.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso) | [SHA256](https://www1.sj.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso.sha256) ||
| Ashburn | [LATEST](https://www1.as.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso) | [SHA256](https://www1.as.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso.sha256) |||
| Ashburn | [LATEST](https://www2.as.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso) | [SHA256](https://www2.as.steamfork.org/images/installer/steamfork-rel-latest-x86_64.iso.sha256) |||

> Note: Release notes are available on the [project's releases page](https://github.com/SteamFork/distribution/releases), however the download files only contain sources.

### Installation
To install SteamFork, flash the bootable image to a USB device and then follow the procedure for your device to boot from removable media.  From the live mode desktop, open the "Install SteamFork" application and then follow the prompts to install to your device.  When complete, close the installer, and shut down the device.  Remove the installation media, and then power the device on to boot into SteamOS.

* SteamFork is compatible with Intel and AMD based systems.  NVidia GPUs are not supported.

## Software
For a full list of verified software, including tools to help set up streaming services, improve power management, and even manage RGB on supported devices, visit the [verified software](https://wiki.steamfork.org/play/verified-software) page on the [SteamFork Wiki](https://wiki.steamfork.org).

## Credits

Like any Linux distribution, this project is not the work of one person.  It is the work of many persons all over the world who have developed the open source bits without which this project could not exist.  Special thanks to Valve for providing SteamOS, HoloISO from which this project originated, ShadowBlip, JELOS, ChimeraOS, and developers and contributors all across the open source community.

## Support
This distribution is made available for myself and others who may want to use it, however it is provided as-is.  Bug fix and feature PRs are always welcome.

## Sources
In addition to sources developed by SteamFork, this project utilizes sources from SteamOS (release repositories), the unofficial Valve source repo, and AUR.

* Valve package repository: `buildroot/pacman-build-*.conf`
* evlaV Repository: https://gitlab.com/evlaV
* Arch AUR repository: https://aur.archlinux.org
* HoloISO (which this project was originally based): https://github.com/HoloISO
