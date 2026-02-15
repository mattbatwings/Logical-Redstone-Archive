# Fractional DectoBin Converter
<img alt="area_render_44_.png" src="images/area_render_44_.png?raw=1" height="300px">

**Authors:** *Xoliks, Flyingdean, Uni, stickman_cookies*

**Endorsed by:** *Waffle [Wueffi]*

**Tags:** *Tested & Functional, Recommended*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472669702164582595)

Converts a Fractional Decimal number into Binary
## Input
n digit value as ss on the top
## Output
n bit value on the side (MSB at the top)
## Speed
2(d-1)+2(p-1)+3rt, (d = # of digits in input, p = degree of precision or # of binary outputs)
## Notes
Infinitely Expandable (7x4x2 per cell), Infinite precision by adding bits to the output, Uses TTP to remove directionality issues. The speed depends on the output size because some numbers would take infinite time to be converted with infinite precision.

## Resources
- [BCDTOBIN003_Fractional_DectoBin_Converter.schem](attachments/BCDTOBIN003_Fractional_DectoBin_Converter.schem): discord
