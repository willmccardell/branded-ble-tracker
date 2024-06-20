# Overview

Reverse Engineering Notes from a BLE tracker I received at a conference.

MCU: 
SOP-8 ST17H68T (probably, the markings have been lasered off)

Exposed pads:
* VDD
* VDD (second one)
* GND
* TMS
* TCK
* PA4

Once booted, the pads have different uses than their name implies. (So no
JTAG...yet)
PA4 is used for the LED
TMS is used for the button.
TCK's use is unknown.

See attached photos for the way it behaves on boot.

The device is likely one-time-programmed, as that's a prominent feature of it
and the corresponding mobile app has no OTA abilities.

# Related links
* SDK for the probable chip: https://github.com/17HXX/ST17H6xT
** The good datasheets: https://github.com/17HXX/ST17H6xT/tree/main/Doc%26Tool
* Mostly empty data sheet: https://www.lenzetech.com/public/store/pdf/jsggs/ST17H68T_BLE_SoC_Datasheet_v1.0_202403.pdf
* Reverse Engineering Efforts
** https://github.com/sylvek/itracing2/issues/5
** https://revspace.nl/AntiLost
