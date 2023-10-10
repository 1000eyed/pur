# Assembly instructions

Treat this manual as a suggestion only. I do not have much experience in soldering, so you may want to deviate from the instructions.

## Assemble the PCB

Make sure you read all the guideline before you begin. The battery connector placement is poor, so you may want to explore other possible options.

### Part list
| #     | name                 | comments                                  |
|-------|----------------------|-------------------------------------------|
| 1     | main PCB             | Order at fabricator of your choice        |
| 1     | Nice!nano v2         | Controller board. Make sure you have enough sockets for all pins. |
| 1     | Nice!view            | Optional display. Should you wish to skip it, you will probably need to modify the case to remove the designated window   |
| 1     | EC11                 | Rotary Encoder through hole style         |
| 38    | 1N4148 - SOD-123     | Diodes                                    |
| 1     | MSK-12C02            | Power switch                              | 
| 1     | JST 1.25mm pitch     | Battery connector, 2pin (optional). I used S2B-PH-K-S(LF)(SN)        |
| 1     | 3.7V LiPo            | Battery (optional)                        |
| 38    | KS33 or KS27         | Gateron Low Profile switches              |
| 38    | Keycaps              | MX-compatible keycaps of your choice      |

- Plug in your nice!nano and flash the firmware and check if it is recognized as an input device by your computer. Randomly short input/output pins with tweezers and check that symbols are output. Do not short GND/VCC/RST/RAW pins!
- Solder the diodes and the power switch to the PCB. There is silkscreen overlap on some diodes, but it should not pose issues, as all the diodes but one are facing one direction. The only diode facing the other way round is encoder push button diode (look bottom right).       
  **Issue #1:** the power switch has incorrect labels on the silkscreen, "Off" and "On" positions are reversed.
- (Optional) Solder the nice!view socket to the PCB. Do not solder the pins to the display yet! You will add the display once the case is ready.
- Solder the nice!nano sockets to the PCB, solder pins to the MCU Here is a [guide](https://nicekeyboards.com/docs/nice-nano/getting-started/) how to do that. Remove the MCU from the PCB.
- (Optional) Solder the battery connector and plug in the battery to check if it works with the MCU.        
  **Issue #2: IMPORTANT!** GND and BAT nets are reversed on this PCB, i.e. the oval pin is connected to GND net. When connecting the battery, make sure that positive battery wire (RED) feeds RAW on nice!nano, and negative wire (BLACK) feeds GND.
- Solder the switches and the encoder. There is no plate to keep switches in place, so take to time to align them properly. I like to put keycaps before soldering and align everything by eye.

  ## Assemble the 3D printed case

  ## Assemble the bent metal sheet case
