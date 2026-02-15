# fastest and smallest possible 1t/port vertical write ports
<img alt="writeports.png" src="images/writeports.png?raw=1" height="300px">

**Authors:** *RCS_33*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472693245036335147)

Description: distributes N inputs(numbers) onto K outputs.

Input: N numbers of any size s. additionally, N K-sized bit vectors at the bottom specifying from which N to pull Data from
Output: K numbers of size s.

Speed:
1) 1t per K/5
2) 1t per N + (1t base from number input or 2t base from selection input at the bottom)

Size:(ceil of fraction)
x = 3-wide tileable per K
z = 4-wide tileable per N
y = 2 * bitwidth + 2 * (bitwidth/8) < (air gaps between bytes)

Use cases:
- insanely useful for all sorts of Memory when you want to write to multiple locations in parallel
- can be used for Schedulers, Ram, Cache and basically any form of Memory. It can let components/clients write in parallel without interfering with each other.

Note:
- due to a design quirk, the output is always 11111111 when nothing is being read, except for every 5th output that is always 0. (this is due to the fact that every 5th input is inverted, but the default state for it is still 11111111 which gets inverted to 00000000)
- it is optimal in speed and size and both bit-width and port-count can be expanded indefinitly
- For Reference, Write ports distribute N->K where the delay scales less with K than it does with N. Use them if K > N. (Hand rule: use write ports when you have more Outputs than inputs)

Schematic Content:
bit-width = 16bit
K = 10
N = 4
*grows towards +x +y +z when pasting*

## Resources
- [OTHERCOMB012_writeports.schem](attachments/OTHERCOMB012_writeports.schem): unknown
