# 32 bit sequential (integer) divider
<img alt="2026-05-03_10.05.09.png" src="images/2026-05-03_10.05.09.png?raw=1" height="300px">

**Authors:** *mcdnldsmngr*

**Endorsed by:** *Waffle [Wueffi]*

**Tags:** *Broken, Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1500422095551725629)

Takes in two binary numbers A (max. 32 bit) and B (max. 31 bit) and returns A // B, A % B, i.e. computes the integer part of A / B and the remainder. It performs non-restoring division, so in every iteration we compute both AQ+B and AQ-B (where AQ is the number stored in the accumulator.), and the sign of the previous iteration decides what result we pick.
## Input
two binary numbers A (max. 32 bit) and B (max. 31 bit)
## Output
A // B, A % B
## Speed
Takes in total roughly 40 seconds from pressing the "clock" button to showing the result.  It takes 11t per bit, so 11t * 32 = 352t = 35.2 seconds, then it does the restoring step, plus additional input & output delays.
## Notes
The adder design that is used is Amino's 3t CCA. This is a modification of my previous design that did not show the remainder, I added the gray circuits and also compacted the control logic a bit. When pasting the schematic, you should probably press the "clock" button once, to make sure everything is correctly resetted.

## Resources
- [DIVIDE007_32bitdiv.schem](attachments/DIVIDE007_32bitdiv.schem): unknown
