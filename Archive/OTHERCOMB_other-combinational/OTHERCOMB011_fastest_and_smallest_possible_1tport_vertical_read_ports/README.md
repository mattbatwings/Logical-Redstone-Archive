# fastest and smallest possible 1t/port vertical read ports
<img alt="readports.png" src="images/readports.png?raw=1" height="300px">

**Authors:** *RCS_33*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472693169832460381)

Description: distributes N inputs(numbers) onto K(numbers) outputs.

Input: N numbers of any size s. additionally N K-sized bit vectors at the bottom specifying from which N to pull Data from
Output: K numbers of size s.

Speed:
1) 1t per N/5
2) 1t per K + (2t base from number input or 1t base from selection input at the bottom)

Size:(ceil of fraction)
x = 3-wide tileable per N
z = 4-wide tileable per K
y = 2 * bitwidth + 3 * (bitwidth/8) < (air gaps between bytes. Note that they are 1 block taller than in typical designs)

Use cases:
- insanely useful for all sorts of Memory when you want to read to multiple locations in parallel
- can be used for Schedulers, Ram, Cache and basically any form of Memory. It can let components/clients read in parallel without interfering with each other. (quad read registers for example)

Note:
- it is optimal in speed and size and both bit-width and port-count can be expanded indefinitely
- For Reference, Read ports distribute N->K where the delay scales less with N than it does with K. Use them if N > K. (Hand rule: use read ports when you have more inputs than Outputs)

Schematic Content:
bit-width = 16bit
K = 10
N = 4
*grows towards +x +y +z when pasting*

## Resources
- [OTHERCOMB011_readports.schem](attachments/OTHERCOMB011_readports.schem): unknown
