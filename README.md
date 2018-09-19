# firmadyne-launcher
This simple script will automate the process of firmware emulation through [firmadyne](https://github.com/firmadyne/firmadyne) and it is very useful when you want to just emulate a firmware without store any kind of emulation logs or information.

The main features of this tool are the following:
- Takes as input a file and try to extract and emulate the firmware inside using the scripts provided by firmadyne.
- Provides a verbose mode with `-v` argument in order to show firmadyne script output 
- Does not use firmadyne database.
- Does not save any file inside firmadyne directory in order to prevent any inconsistency state if used before or after a normal firmadyne execution.

## Installation
1. Following all the steps to install firmadyne as shown [here](https://github.com/firmadyne/firmadyne#setup).
2. Clone this repository and then copy `firmadyne_launcher.sh` inside firmadyne folder.
```bash
git clone https://github.com/mindedsecurity/firmadyne-launcher.git
cp firmadyne-launcher/firmadyne_launcher.sh firmadyne/
chmod +x firmadyne/firmadyne_launcher.sh
```

## Run 
```bash
cd firmadyne
./firmadyne_launcher.sh firmware.zip
```

If you want to try firmadyne and firmadyne-launcher, you can use the following firmwares as test cases:
- [Netgear WNAP320](http://www.downloads.netgear.com/files/GDC/WNAP320/WNAP320%20Firmware%20Version%202.0.3.zip)
- [D-Link DIR-850L](ftp://ftp.dlink.eu/Products/dir/dir-850l/driver_software/DIR-850L_fw_revA1_1-14B07beta_all_en_20170724.zip)
- [Netgear WN604](http://www.downloads.netgear.com/files/GDC/WN604/WN604%20Firmware%20Version%202.0.1.zip)

