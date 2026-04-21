# 32 bit sequential (integer) divider without remainder
<img alt="2026-04-21_18.33.39.png" src="images/2026-04-21_18.33.39.png?raw=1" height="300px">

**Authors:** *mcdnldsmngr*

**Endorsed by:** *Waffle [Wueffi]*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1496205151743119451)

32 bit sequential divider. Takes in two numbers A (max. 32 bit) and B (max. 31 bit) and computes A // B, i.e. the integer part of A divided by B. For example, dividing 7 by 2 returns 3. It uses non-restoring division, so B can only be 31 bit at most.
## Input
two numbers A (max. 32 bit) and B (max. 31 bit)
## Output
A // B, i.e. the integer part of A divided by B
## Speed
It takes 32 cycles on a 11t clock, so 11t * 32 = 352t = 35.2 seconds, no matter what the inputs are.
## Considerations
- The remainder can technically be recovered as well, but sometimes one would have to perform an additional restoring step at the end, so do another addition, but I didnt see a nice way to do this.

## Resources
- [DIVIDE006_32bitdivider.schem](attachments/DIVIDE006_32bitdivider.schem): unknown
