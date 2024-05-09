# SteamFork
SteamFork is a personal project to create an immutable Linux distribution that is as SteamOS like as possible without sacrificing device compatibility.

## Downloads
Downloads are hosted at [SteamFork.org](https://www.steamfork.org/steamfork-images/steamfork-installer/) and updates are available OTA.  A download link to the latest installation ISO can be found below.

### Installation Images
| Branch | URL | Checksum |
| -- | -- | -- |
| Stable | [LATEST](https://www.steamfork.org/steamfork-images/steamfork-installer/steamfork-rel-latest-x86_64.iso) | [CHECKSUM](https://www.steamfork.org/steamfork-images/steamfork-installer/steamfork-rel-latest-x86_64.iso.sha256) |

## Features
* Full SteamOS UI/UX, including desktop mode.
* Power management optimizations ported from [JustEnoughLinuxOS](https://github.com/JustEnoughLinuxOS).
* Improved fan curves on supported devices.
* RGB disabled by default on Ayaneo and Ayn devices.

## Screenshots

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/SteamFork/.github/main/profile/.images/20240507161726_1.jpg"/></td>
    <td><img src="https://raw.githubusercontent.com/SteamFork/.github/main/profile/.images/20240507161721_1.jpg"/></td>
  </tr>
</table>

## Licenses
SteamFork is a Linux distribution that is made up of many open-source components, and each component is provided under its respective license.  Unless otherwise noted, the content of this project itself is made available under the terms of the MIT license.  See [LICENSE](LICENSE) for details.

## Device Support
| Manufacturer | Device | CPU / Architecture | Known Issues |
| -- | -- | -- | -- |
| Atari | VCS | AMD Ryzen R1606G  | None |
| AYANEO | Air / Air Pro | Amd Ryzen 5 5560U / AMD Ryzen 7 5825U | EDID bug sometimes prevents display from working on boot (sleep/resume to correct), and breaks GPU performance mode.|
| AYANEO | Air Plus | Amd Ryzen 7 6800U | None |
| AYANEO | AYANEO 2S | Amd Ryzen 7 7840U | Must enable sleep in firmware<sup>1</sup>. |
| AYANEO | Flip KB | Amd Ryzen 7 7840U | Must enable sleep in firmware<sup>1</sup>. Touch input does not work yet.|
| Ayn | Loki Max | Amd Ryzen 7 6800U | None |

> [!NOTE]
> <sup>1 </sup>New AMD based devices from Ayaneo do not support sleep due to an incorrect firmware setting.  This setting is locked down and must be enabled using a third party helper.  Follow the process from @ChimeraOS to enable sleep [ [here](https://github.com/ChimeraOS/chimeraos/wiki/Community-Guides#enabling-modern-sleep-on-7000-series-amd-hardware) ].

### TDP Control
For tdp management, switch to desktop mode and then install Decky Loader and Simple Decky TDP.
| Source | Installation URL |
| -- | -- |
| [Decky Loader](https://github.com/SteamDeckHomebrew/decky-loader) | ```curl -L https://github.com/SteamDeckHomebrew/decky-installer/releases/latest/download/install_release.sh \| sh``` |
| [Simple Decky TDP](https://github.com/SteamFork/SimpleDeckyTDP) | ```curl -L https://github.com/SteamFork/SimpleDeckyTDP/raw/main/install.sh \| sh``` |

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
