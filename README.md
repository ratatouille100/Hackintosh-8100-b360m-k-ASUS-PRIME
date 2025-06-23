<h1 align="center">
  <br>
  <img src="https://dortania.github.io/OpenCore-Install-Guide/dortania-logo-clear.png" alt="Hackintosh" width="200">
  <br>
  OpenCore EFI for Intel Hackintosh
  <br>
</h1>

<p align="center">
  <strong>A complete OpenCore EFI configuration for ASUS PRIME B360M-K and RX580 based Hackintosh systems</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/OpenCore-1.0.4-success" alt="OpenCore Version" />
  <img src="https://img.shields.io/badge/macOS-10.13~26-informational" alt="macOS Compatibility" />
  <img src="https://img.shields.io/badge/CPU-i3--8100-blue" alt="CPU" />
  <img src="https://img.shields.io/badge/SMBIOS-iMacPro1,1-orange" alt="SMBIOS" />
  <img src="https://img.shields.io/badge/license-BSD_3--Clause-lightgrey" alt="License" />
</p>

<br>

<p align="center">
  <a href="#desktop_computer-specification">Specification</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#apple-compatible-macos-versions">Compatibility</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#gear-how-to-use">Installation</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#books-other-guides">Guides</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#star-credits">Credits</a>
</p>

<br>

## :desktop_computer: Specification

| **Component**    | **Model**                                   |
|------------------|---------------------------------------------|
| CPU              | Intel i3-8100 (8) @ 3.60GHz                 |
| Motherboard      | PRIME B360M-K                               |
| RAM              | 8GB (2x 4GB) Kingston HyperX FURY @ 2666MHz |
| Audio Chipset    | ALC887                                      |
| GPU              | AMD Radeon RX 580 4GB                       |
| OS Disk (SSDM2)  | SSD Kingston NV1 M.2 2280 NVMe PCIe         |
| macOS Version    | 15.5 (24F74) x86_64                         |
| OpenCore Version | 1.0.4                                       |
| SMBIOS           | iMacPro1,1                                  |

<br>

## :apple: Compatible macOS Versions

- High Sierra (10.13.x)
- Mojave (10.14.x)
- Catalina (10.15.x)
- Big Sur (10.16/11.4)
- Monterey (12.1)
- Ventura (13.5)
- Sonoma (14.0)
- Sequoia (15.x)
- Tahoe (26.x)

<br>

## :gear: How to Use

1. Make your USB installer with [**this guide**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
2. Clone the repository and paste the "EFI" directory into your pendrive
3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and
   select **Generate SMBIOS**, as the model select **iMacPro1,1**.
4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic.
   Set MLB (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values.
   Change ROM to your network card's MAC address without the `:` character. [**How to get MAC Address?**](https://www.wikihow.com/Find-the-MAC-Address-of-Your-Computer)
5. Boot it!

> ⚠️ **IMPORTANT**: You CAN NOT use SMBIOS from this repository, it MUST be unique for every macOS installation

<br>

## :books: Other Guides

**If you have any problems with installation or booting your macOS, kernel panics or another system related issue check
OC configuration guide**  
**If something else isn't working properly (for example USB ports, iServices, DRM/Netflix) check Post-Install guide**

- Creating USB installer: [**\*click\***](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
- OpenCore configuration: [**\*click\***](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html)
- Post-Install: [**\*click\***](https://dortania.github.io/OpenCore-Post-Install/)
- Troubleshooting: [**\*click\***](https://dortania.github.io/OpenCore-Post-Install/)
- ACPI patching: [**\*click\***](https://dortania.github.io/Getting-Started-With-ACPI/)
- USB mapping: [**\*click\***](https://dortania.github.io/OpenCore-Post-Install/usb/)

<br>

## :star: Credits

- [[EFI] OpCore-Simplify](https://github.com/lzhoang2801/OpCore-Simplify)
- [[Bootloader] OpenCore](https://github.com/acidanthera/OpenCorePkg)
- [[README.md] Hackintosh-13900k-z790-ASUS-MAXIMUS-HERO](https://github.com/gabrielmaialva33/Hackintosh-13900k-z790-ASUS-MAXIMUS-HERO)

<br>

## :rocket: Contributors

| [![George Kalinin](https://avatars.githubusercontent.com/u/146064808?size=100)](https://github.com/ratatouille100) |
|-------------------------------------------------------------------------------------------------------------------|
| [George Kalinin](https://github.com/ratatouille100)                                                               |

<br/>

<p align="center">&copy; 2025 <a href="https://github.com/ratatouille100" target="_blank">George Kalinin</a></p>
