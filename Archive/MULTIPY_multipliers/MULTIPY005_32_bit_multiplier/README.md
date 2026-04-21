# 32 bit multiplier
<img alt="2026-04-21_10.22.16.png" src="images/2026-04-21_10.22.16.png?raw=1" height="300px">

**Authors:** *mcdnldsmngr*

**Endorsed by:** *Waffle [Wueffi]*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1496185798431739984)

32 bit sequential multiplier, which allows for inputs of up to 32 bits. Note that its maximal output is 33 bit, so in order to ensure that the result is correct, the inputs should not be too large. Example: if A and B are both 16 bit or less, it works without problems. If A is e.g. 28 bit and B is 5 bit, it still works since the result is 33 bit. If A is 28 bit and B is 6 bit however the result will be wrong since it would be 34 bit. This uses the standard shift-and-add algorithm. The adder design that is used is the 3t CCA design by Amino.
## Input
Two binary numbers A,B, can both be 32 bit, but want bit-length(A) + bit-length(B) <= 33 in order to ensure correct result
## Output
33 bit binary product
## Speed
4t per bit of B, plus additional 2t for every 8 bits of B

## Resources
- [MULTIPY005_16bitmult.schem](attachments/MULTIPY005_16bitmult.schem): unknown
