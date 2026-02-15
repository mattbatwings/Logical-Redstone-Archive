# Tristate Register
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472729369951867113)

A versatile tristate register ready to be used in caches or cache less RAM. It is able to (in the right conditions) read and write at 10 Hz, and is more compact than certain traditional registers without much added complexity.
## Input
8-bit data, Read line, Write pulse
## Output
8-bit data
## Speed
2 tick read, 3 tick including standard decoder
## Notes
Read and write lines are inverted (this allows standard glass tower decoders to take one tick). Since this is a tristate register, you cannot read and write at the same time (reading while writing outputs 0). The containers in the schematic which are hoppers must stay that way in order for the glass towers to not be cut off when the register is pasted 2 wide apart (staggered). The barrels can stay as such.

## Resources
- [REGISTER002_tristatereg.schem](attachments/REGISTER002_tristatereg.schem): unknown
