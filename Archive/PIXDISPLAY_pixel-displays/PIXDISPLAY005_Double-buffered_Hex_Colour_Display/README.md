# Double-buffered Hex Colour Display
<img alt="color-screen-front.png" src="images/color-screen-front.png?raw=1" height="300px">

**Authors:** *Uni, Tony*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1539679371512774746)

A double-buffered 16x16 color pixel screen. It takes horizontal and vertical coordinates and a hex number representing a colour, draws pixels into a buffer, can fill the whole buffer with a selected colour, and can draw the buffer to the display. Back buffer is pipelinable at 3 redstone ticks. The screen requires a texture pack that replaces redstone dots with coloured cubes.
## Input
Horizontal and vertical coordinates, plus a hex number representing colour.
## Output
Draws a pixel into a buffer; can fill the whole buffer with a selected colour and then draw the buffer to the display.
## Speed
Pipelinable at 3 redstone ticks.
## Considerations
- Requires a texture pack that replaces redstone dots with coloured cubes.
- Uses specific texture packs: RGB Redstone 2.1 (attached) and a merged version of RGB Redstone 2.1 and Mattpack 1.21 (attached too) for development purposes.
## Notes
Size: 16x16 pixels. Double-buffered. Authors: Uni (base compact design) and Tony (syncing, harness and testing).

## Other Images
<img src="images/color-screen-back.png?raw=1" height="300px">

## Resources
- [PIXDISPLAY005_RGB_Redstone_2.1.zip](attachments/PIXDISPLAY005_RGB_Redstone_2.1.zip): application/zip
- [PIXDISPLAY005_MattPackColoredScreen_1.21.zip](attachments/PIXDISPLAY005_MattPackColoredScreen_1.21.zip): application/zip
- [PIXDISPLAY005_ColorScreenByUniAndTony2.schem](attachments/PIXDISPLAY005_ColorScreenByUniAndTony2.schem): unknown
