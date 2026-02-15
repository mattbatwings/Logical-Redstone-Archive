# choose-n banking arbiter
<img alt="banking-arbiter.png" src="images/banking-arbiter.png?raw=1" height="300px">

**Authors:** *RCS_33*

**Endorsed by:** *Waffle [Wueffi]*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472643720863027313)

Description: 
chooses n true bits out of a k-wide bit vector based on left/right sided priority. 
In Contrast to the normal arbiter, it does *not* guarantee to choose n bits, when at least n bits in the bit vector are set. But its way faster, so when its not that important, you will choose this over the arbiter most of the time

Input:
1) bit vector to choose from
2) bit vector to disable a choosing layer

Output: 
n bit vectors of length k with at most 1 set bit

Speed: (ceil of the fraction)
1) 1t per k/5 (wire delay)
2) 2t per n/4 (no base delay)

Size:
x = 3-wide tileable per k
z = 2-wide tileable per n
y = 6 high

Use Cases:
- Same as normal arbiter, but faster when you don't care about precision

Notes: 
1) since stacking might be confusing, I marked the region to stack with gold blocks
1) the design is optimal in both speed and size. This is the 1st Iteration, but im pretty confident

Schematic Content:
n = 4
k = 10 (2 modules. Each module consists of 4 normal layers and 1 repeater layer)

## Resources
- [OTHERCOMB008_bankingArbiter.schem](attachments/OTHERCOMB008_bankingArbiter.schem): unknown
