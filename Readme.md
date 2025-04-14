# Introduction

Wi-fi smart plugs which I modified and flashed with ESPHome.

* [Aoycocr-x13](Instructions/Aoycocr-x13.md)
* [Houzetek-RF251](Instructions/Houzetek-RF251.md)


## Detech Flash Size

Flash size
Run esptool.py -p COM8 flash_id
device 4016 is W25Q32BV 32 Mb or 4MB

## Initial flashing

ESPHome is running in a dev container.


The devices were initially flashed using [esptool.py](https://github.com/espressif/esptool/).:

`python "E:\IP\Projects\ESP8266\esptool\esptool.py" --chip esp8266 --port COM3 write_flash -fs 2MB -fm dout 0x0 "E:\IP\Projects\ESP8266\esphome\.esphome\build\enbrighten5\.pioenvs\enbrighten5\firmware.bin"`

`python esptool\esptool.py -p COM8 write_flash --erase-all -fs 4MB -fm dout 0x0 Path_to_firmware.bin`


