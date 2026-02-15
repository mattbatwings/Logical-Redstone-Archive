# cancellable priority encoder
<img alt="cancelAblePriority.png" src="images/cancelAblePriority.png?raw=1">

**Authors:** *RCS_33*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472693290150137866)

Description: priority arbiter inspired by CCAs, that can isolate Regions inside the bit vector to not interfere with other regions.

Input:
1) n-wide bit vector "I" representing the elements you want to arbitrate between
2) n-wide bit vector "S" representing the positions to split. 
If a bit in S at index k is set, it represents that bits 0 to k and k+1 to n in I are behaving like separate priority encoders.

Output: 
n-wide bit vector with at most 1 set bit per isolated region. If no bit in S is set, it behaves like a normal left/right sided priority encoder

Speed: (ceil of the fraction)
1) 1t per k/5 (wire delay)
2) 2t

Size:
x = 3-wide tileable per n
z = 5
y = 5

Use Cases:
- useful for lots of nieche stuff, but mainly for forwarding logic(findin the youngest hitting element that is older than some known element)
- understanding the principle opens up a lot of posibillities for other priority stuff

Notes:
1) since stacking might be confusing, I marked the region to stack with gold blocks
1) i *think* the design is optimal in both speed and size

Schematic Contents:
n = 10

## Resources
- [OTHERCOMB013_cancelPriorityEncoder.schem](attachments/OTHERCOMB013_cancelPriorityEncoder.schem): unknown
