# Lucam - CherryCam V1

| ID | Requirement | Reason |
| -- | -- | -- |
| 01 | SoC Raspberry Pi CM4 | Native IMX477 driver |
| 02 | CM4 Connector: Hirose DF40 dual 100-pin mezzanine | Perfect for CM4 |
| 03 | CM4 MIPI CSI-2 interface | Required for IMX477 |
| 04 | Sony IMX477 (12.3 MP, 1/2.3") | Decent res, like an old digicam |
| 05 | MIPI CSI-2 4-lane, up to 1.5 Gbps/lane | Required in datasheet |
| 06 | Sensor connector: 22-pin FFC/FPC 0.5 mm pitch (same as Pi HQ Camera) | following pi hq cam |
| 07 | Sensor power rails: VANA 2.8 V, VDIG 1.8 V, VDDL 1.8 V | Required |
| 08 | MCLK to sensor: 24 MHz via CM4 GPIO | Req too |
| 09 | ILI9341 TFT 2.4", 240×320 px | my screen |
| 10 | SPI up to 40 MHz | CM4 SPI0 or SPI1 |
| 11 | 3.3 V logic, backlight via PWM-controlled MOSFET | Brightness control |
| 12 | full-size or microSD, SDIO 4-bit | JPEG capture target |
| 13 | CM4 SDIO via dedicated pins (not the CM4 boot SD) | Separate from OS storage |
| 14 | QSPI flash: 8 MB minimum, SPI NOR (e.g. W25Q64) | Firmware / config storage |
| 15 | Input power: USB-C 5 V only no battery, no LiPo | Use connected with a powerbank, couldnt think in a good lipo for this |
| 16 | Status LED: 1× green (power), 1× red (capture/busy) | Operational feedback |
| 17 | UART debug header: 4-pin 2.54 mm (TX, RX, GND, 3V3) | Serial console for CM4 |
 