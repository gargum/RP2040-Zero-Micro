# RP2040-Zero Micro
This is a PCB that converts the Waveshare RP2040-Zero in a drop-in replacement for a Pro Micro.

# Pinouts - RP2040-Zero to Pro Micro
5V  ->  RAW     GP4  ->  SDA     GP11 -> P9    GP28 -> P20
3V3 ->  VCC     GP5  ->  SCL     GP12 -> P8    GP29 -> P21
GND ->  GND     GP6  ->  NONE    GP13 -> P7
GP0 ->  TX      GP7  ->  P6      GP14 -> SCLK
GP1 ->  RX      GP8  ->  MISO    GP15 -> MOSI
GP2 ->  P4      GP9  ->  P18     GP26 -> NONE
GP3 ->  P5      GP10 ->  P10     GP27 -> P19

# Instructions & Notes
The solder jumpers on the bottom of the PCB must be connected in order for this to converter to function.
"L" jumpers correspond to a standard Pro Micro footprint, while "R" jumpers correspond to a Pro Micro mirrored horizontally.
All soldering is SMD, meaning the RP2040-Zero is soldered directly to this PCB without any pins.
SMD pin headers are used on the bottom side, opposite the RP2040-Zero, to attach the completed unit to a board.
The RP2040-Zero is to be soldered with its two buttons facing upwards. This obscures the extra connections on the MCU, so if those are needed, wires will need to be attached before the RP2040-Zero is attached to the PCB.
There are two exposed pins, not including the pin connected to the WS2812 LED, that one is able to hand-solder additional connections to.
The RST pin on the Pro Micro is not connected to anything on the RP2040-Zero, meaning the buttons on the MCU itself will need to be used to restart it or to enter the bootloader.
Some projects place an OLED directly above the Microcontroller. If one wishes to do this, make sure one uses removable connections for the OLED rather than permanently soldering it on such that the buttons are accessible.
