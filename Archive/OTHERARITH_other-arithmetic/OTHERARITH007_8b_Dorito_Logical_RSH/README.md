# 8b Dorito Logical RSH
<img alt="Screenshot_2026-07-20_114829.png" src="images/Screenshot_2026-07-20_114829.png?raw=1" height="300px">

**Authors:** *LLucas*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1528869041261903872)

A barrel shifter based on the dorito design that is able to perform a logical right shift in 2 ticks whilst fitting in a 6 wide footprint
## Input
8b value (1ss min), 3b shift value (15ss from lever, 13ss min from decoder)
## Output
8b right shifted value
## Speed
Input value 2t latency, Shift value 3t latency
## Considerations
- This does truncate the bits that have been shifted out
## Notes
This design is inspired off other designs, the original authors of which are unknown.

## Resources
- [OTHERARITH007_8b_Dorito_Logical_RSH_Fix.litematic](attachments/OTHERARITH007_8b_Dorito_Logical_RSH_Fix.litematic): MC 1.20.4, Size 6x24x18 blocks
- [OTHERARITH007_8b_dorito_rsh.schem](attachments/OTHERARITH007_8b_dorito_rsh.schem): unknown
