<!-- Name Card -->
![x260 Hackintosh](https://cardivo.vercel.app/api?name=x260%20hackintosh&description=ThinkPad%20x260%20running%20macOS&image=https://raw.githubusercontent.com/SuhailSherief/ThinkPad-x260-macOS-OpenCore/main/screenshot/pfp.jpeg&backgroundColor=%22272E&pattern=hideout&colorPattern=%231abc9c&opacity=0.05&fontColor=%23eff4f6)
## Specification
Specification | Configuration
----------- | -----------
Processor | Intel Core i7-6500U
Integrated Graphics | Intel HD Graphics 520
Memory | SK-Hynix 8GB DDR4
Storage | 256GB SATA SSD
Wireless Card | Intel AC-8260 Dual Band + Bluetooth
Bootloader | OpenCore
Bootloader Ver. | v1.0.4
## Screenshot
<p align="center">
  <kbd><br>M O N T E R E Y
  <br><br>
  <kbd><img src="https://raw.githubusercontent.com/SuhailSherief/ThinkPad-x260-macOS-OpenCore/ventura/screenshot/main.png"/></kbd></kbd>
<p align="center">
  <kbd><br>B A T T E R Y
  <br><br>
  <kbd><img src="https://raw.githubusercontent.com/SuhailSherief/ThinkPad-x260-macOS-OpenCore/ventura/screenshot/m1.png"/></kbd></kbd>
</p>
<p align="center">
  <kbd><br>S T A T S
  <br><br>
  <kbd><img src="https://raw.githubusercontent.com/SuhailSherief/ThinkPad-x260-macOS-OpenCore/ventura/screenshot/m2.png"/></kbd></kbd>
</p>

### Before you start
Follow dortania guide on how to create a recovery usb for MacOS installation.
You can find the MacOS installation guide at the following link, [`click here`](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/winblows-install.html#downloading-macos)

Remember to generate your own serial number, board serial number, and smUUID before installing macOS. You can do that easily using the OC Auxiliary Tools.

## MacOS
Currently this repo supports `Sonoma`. For anything below that you can use the [original repo](https://github.com/SuhailSherief/ThinkPad-x260-macOS-OpenCore).

> Airportitwlm needs to be replaced according to the OS version used, the latest airportitwlm by default is for Sonoma.
> The current EFI supports Sonoma out of box. Other features are intact.
> To download latest Airportitwlm patch [`click here`](https://github.com/OpenIntelWireless/itlwm/releases)

# Bios
- `Security -> Security Chip`: **Disabled**;
- `Memory Protection -> Execution Prevention`: **Enabled**;
- `Virtualization -> Intel Virtualization Technology`: **Enabled**;
- `Virtualization -> Vt-directed IO`: **Disabled**;
- `Internal Device Access -> Bottom Cover Tamper Detection`: must be **Disabled**;
- `Anti-Theft -> Computrace -> Current Setting`: **Disabled**;
- `Secure Boot -> Secure Boot`: **Disabled**;
- `UEFI/Legacy Boot`: **UEFI Only**;
- `CSM Support`: **No**.

## What's Working?

- QE/CI Intel HD Graphics 520 `BigSur` `Monterey` `Ventura` `Sonoma`
- Power Management `BigSur` `Monterey` `Ventura` `Sonoma`
- Sleep, Shutdown, Restart `BigSur` `Monterey` `Ventura` `Sonoma`
- Audio Speaker & Earphone `BigSur` `Monterey` `Ventura` `Sonoma`
- Bluetooth `BigSur` [`Monterey`](https://github.com/SuhailSherief/ThinkPad-x260-macOS-OpenCore/issues/3) `Ventura`
- Trackpad, Trackball, Gestures `BigSur` `Monterey` `Ventura` `Sonoma`
- Battery Indicator `BigSur` `Monterey` `Ventura` `Sonoma`
- Camera `BigSur` `Monterey` `Ventura` `Sonoma`
- Dock station [`BigSur` `Monterey`](https://github.com/SuhailSherief/ThinkPad-x260-macOS-OpenCore/issues/2) `Ventura` `Sonoma`
- etc

## Credits:
- [Dortania](https://dortania.github.io/OpenCore-Install-Guide/)
- [Simprecicchiani](https://github.com/simprecicchiani)
- [WinLinMacTutorials](https://www.youtube.com/channel/UCR51utxUtFk8OJQP_bBBJsw)
- [Vcyzteen](https://github.com/vcyzteen)
- [r/hackintosh](https://www.reddit.com/r/hackintosh/)
- [r/unixporn](https://github.com/racka98)
- [SuhailSherief](https://github.com/SuhailSherief/ThinkPad-x260-macOS-OpenCore/tree/ventura)