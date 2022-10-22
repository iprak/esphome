# Introduction

Wi-fi smart plugs which I modified and flashed with ESPHome.

* [Aoycocr-x13](Instructions/Aoycocr-x13.md)
* [Houzetek-RF251](Instructions/Houzetek-RF251.md)

ESPHome is running in a dev container.

The devices were initially flashed using [esptool.py](https://github.com/espressif/esptool/).:

`esptool.py --port COM9 write_flash -fs 1MB -fm dout 0x0 Path_to_firmware.bin`
