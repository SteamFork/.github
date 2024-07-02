# SteamFork
SteamFork is a project to create an immutable Linux distribution that is as SteamOS like as possible without sacrificing device compatibility.

## Features
* Full SteamOS UI/UX, including desktop mode.
* Minimal changes to SteamOS to preserve upstream compatibility.
* Power management optimizations ported from [JustEnoughLinuxOS](https://github.com/JustEnoughLinuxOS).
* Improved fan curves on supported devices.
* RGB off by default, will flash on low battery (on supported devices).
* Supports booting from removable media such as usb drives and micro sd cards (64GB minimum).

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
SteamFork is a Linux distribution that is made up of many open-source components, and each component is provided under its respective license.  Unless otherwise noted, the content of this project itself is made available under the terms of the MIT license.  See [LICENSE](LICENSE) for details.

## Device Support
SteamFork is available for a variety of devices including modern desktop and mini PCs that utilize an AMD APU or GPU.  Devices without sponsors are untested may have unknown issues.
| Manufacturer | Product | Sponsor<sup>1</sup> | Known Issues |
| -- | -- | -- | -- |
| Atari | VCS | [Fewtarius](https://github.com/fewtarius) | None |
| AYANEO | 1S | Unsponsored | Unknown |
| AYANEO | 2 | Unsponsored | Unknown |
| AYANEO | 2021 / Pro / Retro Power | Unsponsored | Unknown |
| AYANEO | 2S | [Fewtarius](https://github.com/fewtarius) | Must enable sleep in firmware<sup>2</sup>. |
| AYANEO | Air / Air Pro | [Fewtarius](https://github.com/fewtarius) |EDID bug sometimes prevents display from working on boot (sleep/resume to correct), and breaks GPU performance mode.|
| AYANEO | Air Plus | [Fewtarius](https://github.com/fewtarius) |None |
| AYANEO | Flip DS | Unsponsored | Unknown |
| AYANEO | Flip KB | [Fewtarius](https://github.com/fewtarius) | Must enable sleep in firmware<sup>2</sup>. Touch input does not work yet.|
| AYANEO | Founder Edition | Unsponsored | Unknown |
| AYANEO | Geek | Unsponsored | Unknown |
| AYANEO | Next, Next Pro | Community tested, unsponsored | Unknown |
| Ayn | Loki Max | [Fewtarius](https://github.com/fewtarius) | None |
| Ayn | Loki Zero | Community tested, unsponsored | Unknown |
| GPD | Win 4 | [anthonycaccese](https://github.com/anthonycaccese) | None |
| GPD | Win Mini | Community tested, unsponsored | None |

> [!NOTE]
> <sup>1 </sup> Sponsored devices are fully supported by its maintainer.  Support for unsponsored devices may vary. <sup>2 </sup>New AMD 7000 series devices do not support S3 sleep due to an incorrect firmware setting.  This setting is locked down and must be enabled using a third party helper.  Follow the process from @ChimeraOS to enable sleep [ [here](https://github.com/ChimeraOS/chimeraos/wiki/Community-Guides#enabling-modern-sleep-on-7000-series-amd-hardware) ].

### Documentation
SteamFork documentation is hosted on our [Wiki](https://wiki.steamfork.org).  There you will find answers to [Frequently Asked Questions](https://wiki.steamfork.org/faqs/), [Build](https://wiki.steamfork.org/contribute/build/) and [Device Quirk](https://wiki.steamfork.org/contribute/quirks/) development instructions, and much more.

### Sponsorship
Sponsoring a device is a commitment to maintaining support for your device by validating, testing, and bugfixing any issues that may arise.  Adding support for a device's basic features is straight forward, however, it can become far more technical to add support for features such as fan control.  If you are interested in sponsoring your device, follow the process below.

1. Create a GitHub account if you do not already have one.
2. Boot the SteamFork live image.
3. Create a device quirk using the quirk generator included.  Minimum requirements are gamescope resolution, and rotation if needed.
```
$ sudo -s
# steamfork_quirk_generator --help
```
4. Create a pull request to the [SteamFork Device Support](https://github.com/SteamFork/distribution/tree/main/PKGBUILD/steamfork-device-support) package with your new addition.
5. Open and take ownership of any issues specific to your device on the [SteamFork Bug Tracker](https://github.com/SteamFork/bugtracker).
6. When ready to begin sunsetting support for your device, generate and PR new quirk with the `--supported false` property.

## Downloads 
Downloads are hosted at [SteamFork.org](https://www.steamfork.org/steamfork-images/steamfork-installer/) and updates are available OTA.  A download link to the latest installation ISO can be
 found below.

| Branch | URL | Checksum | Version |
| -- | -- | -- | -- |
| Stable | [LATEST](https://www.steamfork.org/steamfork-images/steamfork-installer/steamfork-rel-latest-x86_64.iso) | [SHA256](https://www.steamfork.org/steamfork-images/steamfork-installer/steamfork-rel-latest-x86_64.iso.sha256) | [![Version](https://img.shields.io/github/release/SteamFork/distribution.svg?color=156C9C&label=&style=flat-square)](https://github.com/SteamFork/distribution/releases/latest) |

> Note: Release notes are available on the [project's releases page](https://github.com/SteamFork/distribution/releases), however the download files only contain sources.

### Installation
To install SteamFork, flash the bootable image to a USB device and then follow the procedure for your device to boot from removable media.  From the live mode desktop, open the "Install SteamFork" application and then follow the prompts to install to your device.  When complete, close the installer, and shut down the device.  Remove the installation media, and then power the device on to boot into SteamOS.

* SteamFork only supports systems with AMD APU/GPUs.

## Power Management / TDP Control
To enable management of the device TDP, switch to desktop mode and then install Decky Loader and Simple Decky TDP.
| Source | Description | Installation URL |
| -- | -- | -- |
| [Decky Loader](https://github.com/SteamDeckHomebrew/decky-loader) | Steam Deck plugin launcher | ```curl -L https://github.com/SteamDeckHomebrew/decky-installer/releases/latest/download/install_release.sh \| sh``` |
| [Simple Decky TDP](https://github.com/SteamFork/SimpleDeckyTDP) | TDP control| ```curl -L https://github.com/SteamFork/SimpleDeckyTDP/raw/main/install.sh \| sh``` |
| [HueSync](https://github.com/honjow/HueSync) | RGB control| ```curl -L https://raw.githubusercontent.com/honjow/huesync/main/install.sh \| sh``` |

## Credits

Like any Linux distribution, this project is not the work of one person.  It is the work of many persons all over the world who have developed the open source bits without which this project could not exist.  Special thanks to Valve for providing SteamOS, HoloISO which this project is based upon, ShadowBlip, JELOS, ChimeraOS, and developers and contributors all across the open source community.

## Support
This distribution is made available for myself and others who may want to use it, however it is provided as-is.  Bug fix and feature PRs are always welcome.

## Sources
This project utilizes sources from SteamOS (release repositories), the unofficial Valve source repo, and AUR.

* Valve package repository: `buildroot/pacman-build-*.conf`
* evlaV Repository: https://gitlab.com/evlaV
* Arch AUR repository: https://aur.archlinux.org
* HoloISO (which this project was based): https://github.com/HoloISO
