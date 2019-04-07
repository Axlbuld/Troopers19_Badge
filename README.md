# Troopers19_Badge
My inoffical collection of Troopers19 Badge Stuff

## ESPTool stuff
* install esptool from https://github.com/espressif/esptool
* check connection and hardware: `esptool.py -p /dev/ttyUSB0 flash_id`
* connect to serial with screen: `screen /dev/ttyUSB0 115200` (exit with CTRL-A K)
* write image: `esptool.py -p /dev/ttyUSB0 write_flash 0x0 flash_4MB.bin

## Micropython stuff
* connect to serial with screen: `screen /dev/ttyUSB0 115200` (exit with CTRL-A K) (or miniterm or minicom or putty or...)
* it seems you need to break the current (menu?) program with `CTRL-C`to go to the `>>>` prompt
### fiddling with files (all commands within Micropython (MP) prompt 
Hint: TAB completion works. so type `os.`and hit TAB to see posibilities
```python
import os
os.listdir()        # see directory /
os.listdir("/apps") # see directory /apps

fs = open("config.json")
fs.read("config.json")
fs.close()
```

## Others Work
* Nice GIST about uploading images: https://gist.github.com/doegox/042c400e19394e6bca4dae70067d4dc3
