# zcfan-openrc
OpenRC init file for zcfan

This is an OpenRC init file for [zcfan](https://github.com/cdown/zcfan).

Prerequisite
- A ThinkPad with fancontrol enabled in thinkpad_acpi module. See *Installation* at [zfscan](https://github.com/cdown/zcfan#Installation).

Dependencies:
- [zcfan](https://github.com/cdown/zcfan) - You can install it [from the AUR](https://aur.archlinux.org/packages/zcfan)

Install:
- Place the file *zcfan* in /etc/init.d and make it executeable:  `chmod +x zcfan`.
- Add the service to your runlevel with `rc-update add zcfan`
- Start the service with `rc-service zcfan start`
