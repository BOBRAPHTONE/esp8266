# RGB Lamp

### Schematic on NodeMCU

![nodemcu rgb-lamp fritzing schematic](https://raw.githubusercontent.com/lvidarte/esp8266/master/examples/rgb-lamp/rgb-lamp.png)

### ESP12E

![esp12e pinout](https://raw.githubusercontent.com/lvidarte/esp8266/master/examples/rgb-lamp/esp12e-pinout.jpg)

#### ESP8266 Bootloader Modes

The bootloader can go into a number of modes depending on the state of GPIOs 0, 2 and 15. The two useful modes are the UART download mode (for flashing new firmware) and the flash startup mode (which boots from flash).

| Mode                             | GPIO 0 | GPIO 2 | GPIO 15 |
|----------------------------------|--------|--------|---------|
| UART Download Mode (Programming) |   0    |   1    |    0    |
| Flash Startup (Normal)           |   1    |   1    |    0    |
| SD-Card Boot                     |   0    |   0    |    1    |

CH_PD (or EN) Chip enable. Should be high for normal operation.

### ESP12E + CP2102 USB-UART converter (Programming Mode)

![esp12e rgb-lamp fritzing schematic programming mode](https://raw.githubusercontent.com/lvidarte/esp8266/master/examples/rgb-lamp/rgb-lamp-esp12e-programming.png)

### ESP12E + CP2102 USB-UART converter (Normal Mode)

![esp12e rgb-lamp fritzing schematic normal mode](https://raw.githubusercontent.com/lvidarte/esp8266/master/examples/rgb-lamp/rgb-lamp-esp12e-normal.png)

