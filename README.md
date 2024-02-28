![PicoFlasher logo](https://raw.githubusercontent.com/X360Tools/PicoFlasher/master/picoflasher.png)

# PicoFlasherZero

Open source XBOX 360 NAND flasher firmware for [Waveshare RP2040-Zero](https://www.waveshare.com/wiki/RP2040-Zero), forked from [PicoFlasher](https://github.com/X360Tools/PicoFlasher)

Tested only on NAND Flash!!!

## Wiring:

### Nand Flash
| Pico | Xbox |
| ------------- | ------------- |
| GP0  | SMC_DBG_EN  |
| GP1  | SMC_RST_XDK_N |
| GP2  | SPI_CLK  |
| GP3  |  SPI_MOSI |
| GP4  |  SPI_MISO |
| GP5  | SPI_SS_N  |
| GND  |  GND |

### ISD12xx Audible Feedback IC (STILL UNTESTED, TRY AT OWN RISK)
|  | Pico | Trinity | Corona |
| ------------- | ------------- | ------------- | ------------- |
SPI_RDY | GP11 | FT2V4 | J2C2-A10
SPI_MISO | GP12 | FT2R7 | J2C2-B11
SPI_SS_N | GP13 | FT2R6 | J2C2-A11
SPI_CLK | GP14 | FT2T4 | J2C2-A8
SPI_MOSI | GP15 | FT2T5 | J2C2-B8

### EMMC Flash (STILL UNTESTED, TRY AT OWN RISK)
| Pico | Xbox | Corona 4GB |
|------| ------------- | ------------- |
| GP6  | FLSH_DATA<0> | U1D1 pin 16 |
| GP7  | FLSH_WP_N (CMD) | U1D1 pin 3 |
| GP8  |  FLSH_CE_N (CLK) | U1D1 pin 2 |
| GP9  |  MMC_RST_N | U1D1 pin 1 |
| GP10 | SMC_RST_XDK_N  | Same as 16MB flash |
| GND  |  GND | U1D1 PIN 4 |

**DO NOT SOLDER ANYTHING TO THE CRYISTAL**
