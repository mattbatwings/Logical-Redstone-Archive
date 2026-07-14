# 32x32 pixel/4x6 sprite display
<img alt="Zrzut_ekranu_2026-07-14_113226.png" src="images/Zrzut_ekranu_2026-07-14_113226.png?raw=1" height="300px">

**Authors:** *MNbiom*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1526534078072098886)

A 32x32 screen that allows you to set pixel to 1 or 0, fill the screen with 1 or 0, and draw a 4x6 sprite at any coordinate. It has a buffer.
## Input
- pixel x (5 bit)
- pixel y (5 bit)
- sprite x (5 bit)
- sprite y (5 bit)
- sprite input (6 nibble)
- draw sprite
- pixel color
- draw pixel
- fill screen
- buffer
## Output
Lamps
## Speed
Draws sprite in 4rt (6 pixels / 1rt)
## Notes
- (0, 0) is in the top left corner.
- Sprite coordinate specifies the bottom left corner of the sprite, so if you want to draw full 4x6 sprite in top left corner, sprite coordinate should be (0, 5).

## Resources
- [CHARDISPLAY003_screen_32x32_4x6_sprite_bottom_left.schem](attachments/CHARDISPLAY003_screen_32x32_4x6_sprite_bottom_left.schem): unknown
