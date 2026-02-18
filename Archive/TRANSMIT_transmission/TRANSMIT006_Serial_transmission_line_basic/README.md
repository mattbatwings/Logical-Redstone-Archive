# Serial transmission line basic
<img alt="serial_render.png" src="images/serial_render.png?raw=1" height="300px">

**Authors:** *Indy*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1473594784076533846)

sends an 8 bit binary number serially over 1 line and 1 clock line.
## Input
8b input, CLK (must be pressed 1x for load, 8x for transmission)
## Output
8b output
## Speed
16RT (2RT per pulse) + 1RT every 15 blocks
## Notes
To load a number, you have to press the clock ONCE, disable the inputs, and then press 8x to transmit.

## Resources
- [TRANSMIT006_8b_serial_transmission.schem](attachments/TRANSMIT006_8b_serial_transmission.schem): unknown
