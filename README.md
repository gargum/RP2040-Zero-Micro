# RP2040-Zero Micro
This is a PCB that converts the Waveshare RP2040-Zero in a drop-in replacement for a Pro Micro.

# Pinouts - RP2040-Zero to Pro Micro

| RP2040-ZERO  | PRO MICRO |
| ------------- | ------------- |
| 5V  | RAW |
| 3V3 | VCC |
| GND | GND |
| GP0 | TX  |
| GP1 | RX  |
| GP2 | P4  |
| GP3 | P5  |
| GP4 | SDA |
| GP5 | SCL |
| GP6 | NONE |
| GP7 | P6 |
| GP8 | MISO |
| GP9 | P18 |
| GP10 | P10 |
| GP11 | P9 |
| GP12 | P8 |
| GP13 | P7 |
| GP14 | SCLK |
| GP15 | MOSI |
| GP26 | NONE |
| GP27 | P19 |

# How to Make/Purchase
In this repository, there is a ZIP file called "RP2040_PRO_ZERO.ZIP". This is the precompiled ZIP file that one uses to order this from PCBWay or JLCPCB.
The contents of this ZIP file can be seen in the RP2040_PRO_ZERO folder in this repository. The ZIP and the folder are simply a collection of gerber files.

On PCBWay, go to the website's home page, then click the "PCB Instant Quote" option in the top bar, before selecting the "Quick-order PCB".
An option should appear on-screen reading, "+ Add Gerber File". Select this option, before uploading the precompiled RP2040_PRO_ZERO.ZIP file. Unzipping it is not necessary.

On JLCPCB, go to the website's homepage then simply click the "Order now" option. 
An option should appear on-screen reading, "Add gerber file". Select this option, before uploading the precompiled RP2040_PRO_ZERO.ZIP file. Unzipping it is not necessary.

# How to Modify
Everything was made using Kicad. No other software was used, nor were any add-ons or extensions used. All of the Kicad files for this project are included in this repository.
Kicad is free software available on any desktop operating system. Kicad does not require one to spend any money at any point in time, don't worry.
If you want to modify this PCB for whatever reason, simply download this repository as a ZIP file, then extract all of that to a folder.
From this folder, you can then simply double-click RP2040_ZERO_REV.kicad_pcb or RP2040_ZERO_REV.kicad, and it will open, allowing you to modify the PCB.

# Instructions & Notes
The solder jumpers on the bottom of the PCB must be connected in order for this to converter to function.
"L" jumpers correspond to a standard Pro Micro footprint, while "R" jumpers correspond to a Pro Micro mirrored horizontally.
All soldering is SMD, meaning the RP2040-Zero is soldered directly to this PCB without any pins.
SMD pin headers are used on the bottom side, opposite the RP2040-Zero, to attach the completed unit to a board.
The RP2040-Zero is to be soldered with its two buttons facing upwards. This obscures the extra connections on the MCU, so if those are needed, wires will need to be attached before the RP2040-Zero is attached to the PCB.
There are two exposed pins, not including the pin connected to the WS2812 LED, that one is able to hand-solder additional connections to.
The RST pin on the Pro Micro is not connected to anything on the RP2040-Zero, meaning the buttons on the MCU itself will need to be used to restart it or to enter the bootloader.
Some projects place an OLED directly above the Microcontroller. If one wishes to do this, make sure one uses removable connections for the OLED rather than permanently soldering it on such that the buttons are accessible.

# License - Mystery Box
This product uses a mystery box license. One's rights regarding the use of this PCB, including whether or not it is even open source, are a secret.
In order to learn what one is allowed to do with this PCB, one must ask the creator directly, who must then physically mail a tiny colourful box with the answer inside it.
