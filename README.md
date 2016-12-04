# autoreboot
A debian package (.deb) to automatically check if reboot is required when network is unavailable. (for HSA)

## Introduction
This is a package that runs a daemon to automatically check if the system is reboot-required. The reboot condition is set to be when network is not available. This package is especially helpful for HSA-compatiable machines because such machines often suffer from suddenly broken IOMMU. It would be very inconvenient if network becomes unavailable on some occasion that the user is accessing the machine via a remote connection. This package also provide commands to manually enable/disable automatic reboot checking.

## Installation
Download the package from the [release page](https://github.com/cyliang/autoreboot/releases) and install it with `dpkg`.
```sh
% dpkg -i autoreboot*.deb
```

### Uninstall
It is very easy to uninstall this package:
```sh
% dpkg --purge autoreboot
```
