# 1 KiB ROM with Cache (expandable)
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *LLucas*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472659629887717439)

A cached read only memory designed to hold CPU instructions
## Input
Page swap address, Address within cache
## Output
Values stored in barrels
## Speed
7 tick read, 10 word/sec swap
## Considerations
- Putting the desired values in the barrels is kind of janky, you might have to mess with the hex to bin converter to see how it inputs the data into the ROM.
## Notes
Page size: 32 word / 64 Byte. Main memory: 16 pages / 1 024 Byte. Main memory size: 2 blocks/bit.

## Resources
- [ROM002_1KiBROM_1.schem](attachments/ROM002_1KiBROM_1.schem): unknown
