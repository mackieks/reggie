# reggie

A tiny, powerful open source regulator board based on TPS563203DRLR. Reggie is perfect for replacing PTH08080s in designs both old and new!

![P1c6E5o9](https://github.com/user-attachments/assets/ca140b02-1caa-46df-8dc6-3e58651c6987)

Specs:

- Tiny 8.5 x 10.8mm PCB
- 4.2V to 17V input (14V recommended maximum)
- 0.6 to 7V output
  - set Vout with 1206 size resistor on underside of board
- 3A max output current
  - thermally limited— at voltages &gt;5V, output current is lower
- 80% or better efficiency

Usage:

- Solder a 1206 size resistor to the footprint on the bottom of the PCB to set Vout. (With no resistor, Vout is 0.6V.)
  - 1V - 18k
  - 1.15V - 13k
  - 1.5V - 7.5k
  - 1.8V - 5.9k
  - 2.5V - 3.74k
  - 3.3V - 2.61k
  - 3.5V - 2.49k
  - 5V - 1.58k
- The regulator is enabled by default. Connect the EN pin to GND to disable the regulator.&nbsp;
- Reggie does not need external capacitors. However, some applications may benefit from external electrolytic caps.
