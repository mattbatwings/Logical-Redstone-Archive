# Tangent Lookup Table
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *LLucas*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472738030237253704)

A lookup table preprogrammed to calculate the tangent of an angle (given in radians). Angle range 0 to 255/128 (1.992) radians.
## Input
8 bit angle - unsigned 1.7 fixed point, radians
## Output
8 bit value - signed 4.4 fixed point
## Speed
9 ticks
## Notes
Angle is in RADIANS! For large positive/negative values, the output value is clamped to either the largest positive or negative value.

## Resources
- [OTHERARITH003_tanlut.schem](attachments/OTHERARITH003_tanlut.schem): unknown
