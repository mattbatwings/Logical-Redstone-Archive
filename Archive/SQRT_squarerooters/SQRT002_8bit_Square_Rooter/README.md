# 8bit Square Rooter
<img alt="17711292643154465268931961841064.png" src="images/17711292643154465268931961841064.png?raw=1" height="300px">

**Authors:** *SafetyIWisher*

**Endorsed by:** *mattbatwings*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1472462338887258315)

8-bit sequential square root extractor
## Input
8-bit Number, Extraction Button
## Output
4-bit Square Root, 5-bit Remainder
## Speed
Total of 71 rTicks after button press
## Notes
Once the button is pressed, it takes 2 ticks to initiate the circuit. The Square Root is saved 4 rTicks after the Remainder, and the circuit is cleared for 1 cycle, 1 rTick after the Root is saved. 1 cycle lasts 13 rTicks, so it takes 8t for init, 4 clock cycles, and 11 ticks to finish saving and clearing. This uses a Non-restoring / trial subtraction Binary Digit-by-Digit Square Root Algorithm.

## Other Images
<img src="images/17711292814353450082511174444754.png?raw=1" height="300px">

<img src="images/17711292925238959991834742815253.png?raw=1" height="300px">

## Resources
- [SQRT002_8bit_seq_sqrt_71rt.schem](attachments/SQRT002_8bit_seq_sqrt_71rt.schem): unknown
  - WorldEdit Schematic
