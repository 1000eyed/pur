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

  ### Part list
| #     | name                                 | comments                                  |
|-------|--------------------------------------|-------------------------------------------|
| 1     | 3D printed keyboard case             | Order at fabricator of your choice        |
| 6     | Heat inserts                         | M2x4x3.5                                  |
| 6     | Hex bolts                            | M2x4                                      |
| 10    | Magnets                              | Cylindrical 2x4mm                         |
| 5     | Adhesive silicon feet                | 10mm                                      |
| drop  | Superglue                            |                                           |
| small strip  | two sided adhesive tape       |                                           |

- Drive heat inserts into designated holes on the top case using a solder iron.
- Insert magnets to the both case parts, securing them with superglue. Mind polarity, so that the case closes.
- Attach 4 rubber feet to the bottom case.
- Glue one silicon leg next to nice!view socket. This will stabilize the display so that it does not fall into the case under pressure.
- Drive the pins out of the socket header which came with nice!view and insert them into the sockets on the PCB. Do not solder the display yet.
- Attach the PCB to the top case with bolts and close the case.
- Now carefully insert the nice!view into the case window (it will fit snug) and solder the pins.
- Plug in the battery and attach it to the case or PCB with a strip of adhesive tape.

  Turn on and enjoy your PUR!

  ## Assemble the bent metal sheet case

  ### Part list
| #     | name                                 | comments                                  |
|-------|--------------------------------------|-------------------------------------------|
| 1     | Metal sheet case frame               | Order at fabricator of your choice        |
| 6     | Standoffs                            | M2 5mm height                             |
| 6     | Hex bolts                            | M2x10                                     |
| 1     | Adhesive silicon feet                | any size                                  |
| small strip  | two sided adhesive tape       |                                           |

- Glue one silicon leg next to nice!view socket. This will stabilize the display so that it does not fall into the case under pressure.
- Drive the pins out of the socket header which came with nice!view and insert them into the sockets on the PCB. Do not solder the display yet.
- Attach the PCB to the case with bolts and standoffs.
- Now carefully insert the nice!view into the case window (it will fit snug) and solder the pins.
- Plug in the battery and attach it to the case or PCB with a strip of adhesive tape.

  Turn on and enjoy your PUR!
