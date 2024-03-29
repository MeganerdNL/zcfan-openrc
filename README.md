# zcfan-openrc
OpenRC init file for [zcfan](https://github.com/cdown/zcfan).

## Prerequisites / Dependencies:
- A ThinkPad running linux with OpenRC as init system.
- Fancontrol enabled in *thinkpad_acpi* module. See *Installation* at [zcfan](https://github.com/cdown/zcfan#Installation).
- [zcfan](https://github.com/cdown/zcfan) installed - You can install it [from the AUR](https://aur.archlinux.org/packages/zcfan) if you use (an) Arch (based distribution).

## Installation:
#### From the [AUR](https://aur.archlinux.org/packages/zcfan-openrc)
- `yay -S zcfan-openrc` - or with your own favorite AUR helper.
- Add the service to default runlevel with `rc-update add zcfan`
- Start the service with `rc-service zcfan start`
#### Manual
- Place the file *zcfan* from this repository in */etc/init.d* and make it executable: `chmod +x zcfan`.
- *Optionally* create a file */etc/zcfan.conf* with your temperature values (in °C) for low, medium and maximum fan speed:
```
max_temp 90
med_temp 80
low_temp 70
```
- Add the service to default runlevel with `rc-update add zcfan`
- Start the service with `rc-service zcfan start`

## Further documentation:
See [zcfan](https://github.com/cdown/zcfan).
