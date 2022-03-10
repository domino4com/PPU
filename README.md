<img src="assets/PPU.svg" width=200 align="right">

# PPU Power Programmer USB-A
PPU Power Programmer USB-A


## Power
- 3.3v is provided on ```Vcc``` from an *AMS1117-3.3 Voltage Regulator*.
- Original 5v from USB is prvided on ```Vsrc```
- This provides 1A (1000mA) of current to your circuit.
- A blue LED is permanently lit when power is avaliable.
- You can download the datasheet from [Advanced Monolithic Systems](http://www.advanced-monolithic.com/pdf/ds1117.pdf)


## Programmer
- This module contains a *CH340x USB to Serial Converter* chip.
- You can download datasheet and drivers from [WinChipHead (WCH)](http://www.wch-ic.com/search?q=CH340&t=downloads).
- :warning: Unlike what is stated in the datasheet, this converter chip cannot use a transfer speed of 921600 bps. Maximum transfer speed in Arduino is 460800 bps. However if you use a tool where you can specify transfer speed, such as the [ESPTOOL](https://github.com/espressif/esptool), then you can also use a transfer speed of 1000000 bps.
  - https://github.com/espressif/esptool/issues/435

## Troubleshooting
- Install Arduino first. Arduino installs drivers for most boards in most operating systems. Download [Arduino](https://www.arduino.cc/en/software)
- If you still have issues seeing your serial port, then install drivers from [WinChipHead (WCH)](http://www.wch-ic.com/search?q=CH340&t=downloads).
