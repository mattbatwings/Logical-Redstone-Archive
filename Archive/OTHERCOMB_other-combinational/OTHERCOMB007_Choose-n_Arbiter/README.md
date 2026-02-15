# Choose-n Arbiter
<img alt="arbiter.png" src="images/arbiter.png?raw=1" height="300px">

**Authors:** *RCS_33*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472643663023706303)

Chooses n true bits out of a k-wide bit vector based on left/right sided priority. 
if there are at least n set bits in the vector, the arbiter *guarantees* to choose n of them

Input:
1) bit vector to choose from
2) bit vector to disable a choosing layer

Output: 
n bit vectors of length k with at most 1 set bit

Speed: (ceil of the fraction)
1) 1t per k/5 (wire delay)
2) 2t per n (no base delay)

Size:
1) 3-wide tileable per k
2) 4-wide tileable per n
3) 5 high

Use cases:
-> comes in handy when wanting to choose multiple entries in a set recursively to convert some of the bandwidth to througput
-> if you want to design OoO Cores, you will properbly need this a *lot*

Notes: 
1) since stacking might be confusing, I marked the region to stack with gold blocks
1) the design is optimal in both speed and size. This is the 5th Iteration, trust me.
(There is also a Vertical Version with equal Timings)

Schematic Content:
n = 4
k = 10 (2 modules. Each module consists of 4 normal layers and 1 repeater layer)

## Other Images
<img src="images/arbiterVertical.png?raw=1" height="300px">

## Resources
- [OTHERCOMB007_arbiter.schem](attachments/OTHERCOMB007_arbiter.schem): unknown
- [OTHERCOMB007_arbiterVertical.schem](attachments/OTHERCOMB007_arbiterVertical.schem): unknown
