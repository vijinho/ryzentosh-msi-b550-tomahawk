# Opencore Ventura EFI - Ryzen 5600, RX6600, MSI B550 TOMAHAWK MAG Motherboard

This is built on the work of many others, too numerous to mention, thanks to all, and I am sharing this back with the community. It is triple-booting on a system shared with Windows 10, Linux (PopOS using BTRFS filesystem).

## Hardware tested

- Motherboard: MSI MAG B550 Tomahawk ATX (with Resize Bar/Above 4G Enabled)
- CPU: Ryzen 5 5600
- Graphics Card: MSI AMD RX 6600
- Wireless/Bluetooth: Genuine Apple BCM94360 used in a PCIe x1 add-in card

No serious issues detected, other than not sleeping.
 
## Notes

- `config.plist` is excluded, you need to copy the example `config-ryzen-msi-b550.plist` and replace the asterisks with generated valid ROM etc values
- Power monitoring app can be added from Truly Spinach [SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor) but the kernel files are included already.

## Help

Don't create issues asking, but do send patches and pull requests for improvements! For self-help. refer to:

- [OpenCore Configurator ](]https://mackie100projects.altervista.org/)
- [Dortania Guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [mikigal/ryzen-hackintosh]https://github.com/mikigal/ryzen-hackintosh
- [Github Ryzentoshers](https://github.com/topics/ryzen-hackintosh)

## Scripts

### Ryzen Patches

Run
```
scripts/ryzen-patch.sh
```

### Setting your computer/hostname

Run
```
scripts/hostname.sh COMPUTERNAME
```

### Constant iCloud/AppStore Popups
If you run into problems with being asked constantly about your iCloud information, try deleting network interfaces and then restarting after typing the following in a terminal:

```
scripts/clear-network-interfaces.sh
```

