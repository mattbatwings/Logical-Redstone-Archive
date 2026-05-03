# Slow 32 bit (integer) square root
<img alt="2026-05-03_11.00.35.png" src="images/2026-05-03_11.00.35.png?raw=1" height="300px">

**Authors:** *mcdnldsmngr*

**Endorsed by:** *Waffle [Wueffi]*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1500433872863756348)

Takes a binary number A (max. 32) bit and returns the integer part of sqrt(A) as well as the remainder, e.g. sqrt(11) would be 3 with remainder 2. Uses the shift-and-add algorithm featured in Mattbatwings' video with Amino's 3t CCA. By doing more iterations, can obtain bits after the decimal point up to 16 bits.
## Input
binary number A (max. 32 bit)
## Output
integer part of sqrt(A) as well as the remainder
## Speed
18t per bit, so 18t * 16 = 288t = 28.8 seconds, plus input & output delay, so in total roughly 30 seconds
## Considerations
- Uses conditional subtractor, quite slow
- Non-restoring algorithm could push down to at least 11t per bit
## Notes
CCA design that is used is Amino's 3t CCA. By increasing the time length of the capacitor at the bottom, could compute the square root up to 16 bits after the decimal point.

## Resources
- [SQRT006_32bitsqrt.schem](attachments/SQRT006_32bitsqrt.schem): unknown
