# SteamFork
SteamFork is a personal project to create an immutable Linux distribution that is as SteamOS like as possible without sacrificing device compatibility.

## Downloads
Downloads are hosted at [SteamFork.org](https://www.steamfork.org/steamfork-images/steamfork-installer/) and updates are available OTA.  A download link to the latest installation ISO can be found below.

SteamFork Installation Image: [ [LATEST](https://www.steamfork.org/steamfork-images/steamfork-installer/steamfork-rel-latest-x86_64.iso) ] [ [CHECKSUM](https://www.steamfork.org/steamfork-images/steamfork-installer/steamfork-rel-latest-x86_64.iso.sha256) ]

## Licenses
SteamFork is a Linux distribution that is made up of many open-source components, and each component is provided under its respective license.  Unless otherwise noted, the content of this project itself is made available under the terms of the MIT license.  See [LICENSE](LICENSE) for details.

## Device Support
| Manufacturer | Device | CPU / Architecture | Known Issues |
| -- | -- | -- | -- |
| Atari | VCS | AMD Ryzen R1606G  | None |
| AYANEO | Air / Air Pro | Amd Ryzen 5 5560U / AMD Ryzen 7 5825U | None |
| AYANEO | Air Plus | Amd Ryzen 7 6800U | None |
| AYANEO | AYANEO 2S | Amd Ryzen 7 7840U | Display does not turn off during sleep. |
| Ayn | Loki Zero | AMD Athlon Silver 3050e | None |
| Ayn | Loki Max | Amd Ryzen 7 6800U | None |

## Credits

Like any Linux distribution, this project is not the work of one person.  It is the work of many persons all over the world who have developed the open source bits without which this project could not exist.  Special thanks to Valve for providing SteamOS, HoloISO which this project is based upon, ShadowBlip, JELOS, and developers and contributors all across the open source community.

## Support
This distribution is made available for myself and others who may want to use it, however it is provided as-is.  Bug fix and feature PRs are always welcome.

## Sources
This project utilizes sources from SteamOS (release repositories), the unofficial Valve source repo, and AUR.

* Valve package repository: `buildroot/pacman-build-*.conf`
* evlaV Repository: https://gitlab.com/evlaV
* Arch AUR repository: https://aur.archlinux.org/
* HoloISO (which this project was based): https://github.com/HoloISO
