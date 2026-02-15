# 2t/port 3-wide CAM
<img alt="CAM.png" src="images/CAM.png?raw=1" height="300px">

**Authors:** *RCS_33*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472693123351187586)

Description: multi-ported CAM. compares every element in some Set with every other element in another Set and outputs a binary hit Matrix

Input: 2 Sets of Numbers, call them A(of size N) and B(of size K)
Output: N x K Binary bit Matrix where every element(1 bit) at index {i,j} specifes if element i in A and j in B are equal.

Speed:
1) Speed of A: 2t per K
2) Speed of B: 1t per N/5

Size: (ceil of fraction)
x = 3-wide tileable per N
z = 9-wide tileable per K
y = 2*bitwidth+2*(bitwidth/8)

Use Cases:
- Useful for Caches, Ram etc. For example, you could swap cache lines without halting the CPU since you can read/write in parallel through ports

Note:
- properbly optimal in time, but idk about size. Anyway, properbly good enough for everything you ever need
- normally, youd connect your Memory to compare against in A and the values you want to search with in B

Schematic Content:
16-bit
N = 10
K = 4

## Resources
- [OTHERCOMB010_CAM.schem](attachments/OTHERCOMB010_CAM.schem): unknown
