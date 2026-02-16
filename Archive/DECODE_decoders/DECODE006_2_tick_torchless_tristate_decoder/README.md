# 2 tick torchless tristate decoder
<img alt="screenshot_1.png" src="images/screenshot_1.png?raw=1" height="300px">

**Authors:** *LLucas*

**Endorsed by:** *Waffle [Wueffi]*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1473018624896794706)

A decoder where if 15 ss is inputted into the decoder, it acts as a normal decoder, however, inputting 14ss onto all bits enables all outputs. You can also customize which bits are marked as "don't care" by inputting 14ss onto separate layers.
## Input
3 bit tri-state value.
15ss -> Bit on
14ss -> Don't care
0ss -> Bit off
## Output
8 binary values
## Speed
2 ticks, 1 tick inverted output
## Notes
Thanks to Uni for the idea for this decoder as well as some of the wiring tricks were "borrowed" :P.

You can also remove a part of the decoder in order to get the 1 tick inverted output if that is useful.

## Resources
- [DECODE006_torchlesstristatedecoder.schem](attachments/DECODE006_torchlesstristatedecoder.schem): unknown
