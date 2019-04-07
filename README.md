# Troopers19_Badge
My inoffical collection of Troopers19 Badge Stuff


* install esptool from https://github.com/espressif/esptool
* check connection and hardware: `esptool.py -p /dev/ttyUSB0 flash_id`
* connect to serial with screen: `screen /dev/ttyUSB0 115200` (exit with CTRL-A K)
* write image: `esptool.py -p /dev/ttyUSB0 write_flash 0x0 flash_4MB.bin
