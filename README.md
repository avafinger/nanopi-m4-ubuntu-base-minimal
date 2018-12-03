# nanopi-m4-ubuntu-base-minimal

Ubuntu 18.04 base minimal image for RK3399 (NanoPi M4 / NEO4)


OS Image for development with the following tidbits:

* Kernel 4.4.y (with the best of both world, rockchip bsp kernel + kernel.org 4.4.y)
* Gbps
* Wifi
* Bluetooth
* 3D mali gpu (fbdev / lxde)
* VPU (X11 / lxde)
* camera (WiP)

You need *wget* and *curl* installed to grab the files in a Linux distro.

Get the files by running:


	wget $(curl -s https://api.github.com/repos/avafinger/nanopi-m4-ubuntu-base-minimal/releases/latest | grep -oP '"browser_download_url": "\K(.*)(?=")')


then

	sudo ./flash_sdcard.sh /dev/sdX


# Release v1.0

These are the raw files for building the OS Image with kernel 4.4.166-rockchip