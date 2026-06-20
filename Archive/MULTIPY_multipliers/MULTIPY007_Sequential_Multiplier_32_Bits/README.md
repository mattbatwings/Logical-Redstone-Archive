# Sequential Multiplier (32 Bits)
<img alt="32b_Multiplier.png" src="images/32b_Multiplier.png?raw=1" height="300px">

**Authors:** *Flyingdean, aminotreal*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1517920589686374510)

Multiplies two 32b values together sequentially using peasant multiplication (shift and add).
## Input
Two 32b values, Clock, Clear
## Output
64b product
## Speed
32s [320rt, 640gt] for worst case. Uses a 4rt (+2rt per byte) loop
## Notes
Based on Aminotreal's 16b stackable CCA. Can be downsized with little modification.

## Acknowledgements:
- aminotreal: Author of the 16b CCA this design is based on

## Resources
- [MULTIPY007_Flyingdeans_32b_multiplier.schem](attachments/MULTIPY007_Flyingdeans_32b_multiplier.schem): unknown
- [MULTIPY007_Flyingdeans_32b_multiplier.litematic](attachments/MULTIPY007_Flyingdeans_32b_multiplier.litematic): MC 1.21.11, Size 13x130x9 blocks
