# Hackintosh your Deskmini310

## Configuration

| Specifications | Detail                                                                                    |
|----------------|-------------------------------------------------------------------------------------------|
| CPU            | INTEL I7-8700                                                                             |
| RAM            | ADATA DDR4 2666MHz 16GB × 2                                                               |
| SSD            | WD SN750 512GB M.2 PCIE                                                                   |
| WIFI/BT        | BCM94360CS2                                                                               |
| Cooler         | ID-COOLING IS40x                                                                          |

## BIOS

version：P3.4（support P4.x）

* Advanced
  * Chipset Configuration
    * Onboard HD Audio: Enabled
  * USB Configuration
    * XHCI Hand-off: Enabled
  * Super IO Configuration
    * Serial Port: Disabled  
* Security
  * Secure Boot: Disabled(by default)

Other Configurations by default

## Works

* [x] Ethernet/WIFI/Bluetooth/Audio/USB&EX-USB/Sensors

* [x] DP/HDMI dual monitor output

* [x] Shutdown、Sleep

## Notes

* After macOS installed done ([Installation Guide](https://www.tonymacx86.com/threads/unibeast-install-macos-mojave-on-any-supported-intel-based-pc.259381/)), please open `config.plist` and  fill few SMBIOS info by Clover Configurator.

* If you use `BCM94352Z` , please move BCM94352Z/* to CLOVER/kexts/Other.

* If you need to move CLOVER/kexts/Other/* to /L/E&/S/L/E, please modify `InjectKexts` to `Detect` in `config.plist` by Clover Configurator.

## Tips

* If you use `Chrome` , it is recommended to turn off `Chrome` completely when using `IGPU` operations(PS/FCP etc).[Chrome causing Final Cut Pro X to slow down, freeze, and crash](https://appleinsider.com/articles/19/06/20/chrome-causing-final-cut-pro-x-to-freeze-and-crash)

* I will write some detailed tutorials (How to install macos and configure clover, etc.) in my free time, and this repository will be continuously updated until I  use the Deskmini310 no longer.

## Issues

Occasionally restart, but I think this is an inevitable problem for Hackintosh , Fortunately, it happens very rarely.

## Why Hackintosh

Because We Can！

## ChangeLog

| Date      | Content                                                              |
|-----------|----------------------------------------------------------------------|
| 2019.7.28 | update clover  5018 & upgrade Mojave 10.14.6（Supplemental update has not been tested） , everything is alright |
| 2019.7.31 | update clover  5033                                                  |
| 2019.8.7  | upgrade Mojave 10.14.6 Supplemental update.(I restarted automatically several times after upgraded, and everything worked fine now) |
| 2019.8.11 | update clover  5045                                                  |
