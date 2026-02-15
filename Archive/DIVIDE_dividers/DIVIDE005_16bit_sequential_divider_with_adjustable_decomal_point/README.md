# 16bit sequential divider with adjustable decomal point
<img alt="screenshot.png" src="images/screenshot.png?raw=1" height="300px">

**Authors:** *MNbiom*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472589085699735753)

Its an 16bit sequential divider with adjustable decimal point. So you can set whether is should calculate 16.0 or 15.1 ... or 1.15 (integer.fraction (amount of bits))
## Input
A(16bit), B(16bit), amount of fractional bits(hex), button to start(9rt pulse)
## Output
A/B, A%B
## Speed
9rt/bit + initial 7rt (151rt for 16.0(best case); 286rt for 1.15(worst case))
## Notes
A%B output sometimes outputs 1rt pulse, so you might have to filter it with a torch or a comparator

## Resources
- [DIVIDE005_16bit_divider_offset.schem](attachments/DIVIDE005_16bit_divider_offset.schem): unknown
