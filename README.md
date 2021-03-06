# espruna-wd
Remix [espurna-h PCB](https://github.com/xoseperez/espurna-board)

I didn't need current metering HLW8012, however needed an increase in reliability.

I used the [xoseperez](https://github.com/xoseperez) design to make the board using the Watch Dog hardware.

Changes:
- Added hardware Watch Dog timer circuit STMicroelectronics STWD100. It is possible to use pin-to-pin analogs. Pin Enable has 2 pull-up options. Enabled by a jumper.
- 3mm mounting holes (Little space, but dimensions are preserved).
- Slightly changed the layout of the board, redrawn all the tracks of the PCB.
- More GPIOs brought out.

# Watchdog Notes:
- Please use the jumper (pin enable) to disable WD while flashing and configuring the device. Otherwise, you will get flickering.
- Please use STWD100xY (eg WNY marking) with a timeout period of 1.6s (1.12 - 2.24s). Otherwise, the ESP8266 may not boot up in time and you will get flickering.

## Open Hardware

Hardware designs (schematics and CAD) files are licensed under the [Creative Commons Attribution-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0/) and follow the terms of the [OSHW (Open-source hardware) Statement of Principles 1.0.](http://freedomdefined.org/OSHW)

## Disclaimer

THIS PRODUCT IS TARGETED TO EXPERIENCED USERS AT THEIR OWN RISK. THIS PRODUCT IS MEANT TO BE USED PLUGGED TO MAINS AND IT REQUIRES A DEEP UNDERSTANDING OF THE PERILS OF HIGH VOLTAGE ON HUMAN LIFE.

TO THE FULLEST EXTENT PERMISSIBLE BY THE APPLICABLE LAW, I HEREBY DISCLAIM ANY AND ALL RESPONSIBILITY, RISK, LIABILITY AND DAMAGES ARISING OUT OF DEATH OR PERSONAL INJURY RESULTING FROM ASSEMBLY OR OPERATION OF THIS PRODUCT.

