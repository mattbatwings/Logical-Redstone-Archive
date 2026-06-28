# Sequential Divider (32 Bits, Adjustable Radix Point)
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *Flyingdean, aminotreal*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1520813298704978193)

Divides two 32b values together sequentially using repeated subtraction. The number of resultant significant bits can be adjusted using the precision lectern.
## Input
Two 32b values, Clock, Reset, Precision
## Output
Varies based on the Output Setting [Min: 8b, Max: 120b]
## Speed
13n+0.2s [130n+22rt, 260n+22gt] (n represents the selected precision.) Uses a 16rt loop.
## Considerations
- Uses a 16rt loop.
- Overflow errors can sometimes occur when B > A >= 2^31 while using decimal precision so it is recommended to only use 31 bits for B in this case.
- It is recommended to use Page 4 for integer outputs and Page 8 for decimal precision.
## Notes
Based on Aminotreal's 16b stackable CCA.

## Acknowledgements:
- aminotreal: Author of the 16b CCA this design is based on

## Resources
- [DIVIDE010_Flyingdeans_32b_divider_Page_8.schem](attachments/DIVIDE010_Flyingdeans_32b_divider_Page_8.schem): unknown
- [DIVIDE010_Flyingdeans_32b_divider_Page_4.litematic](attachments/DIVIDE010_Flyingdeans_32b_divider_Page_4.litematic): MC 1.21.11, Size 13x67x12 blocks
- [DIVIDE010_Flyingdeans_32b_divider_Page_4.schem](attachments/DIVIDE010_Flyingdeans_32b_divider_Page_4.schem): unknown
- [DIVIDE010_Flyingdeans_32b_divider_Page_8.litematic](attachments/DIVIDE010_Flyingdeans_32b_divider_Page_8.litematic): MC 1.21.11, Size 13x131x12 blocks
- [DIVIDE010_image.png](attachments/DIVIDE010_image.png): image/png
