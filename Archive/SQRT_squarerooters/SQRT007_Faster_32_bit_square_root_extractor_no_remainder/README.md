# Faster 32 bit square root extractor (no remainder)
<img alt="2026-08-15_18.13.45.png" src="images/2026-08-15_18.13.45.png?raw=1" height="300px">

**Authors:** *mcdnldsmngr*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1538226492578726009)

A device that takes a 32-bit number A as input and returns floor(sqrt(A)) using a non-restoring algorithm.
## Input
A 32 bit number A.
## Output
floor(sqrt(A)) (the square root of A rounded down).
## Speed
Runs on a clock speed of 11rt per bit. Due to overhead, it needs a little over 20 seconds in total.
## Considerations
- No remainder. The remainder is stored on the yellow part in the middle of the unit, which is hard to access. Also, we sometimes have to perform an additional step at the end to obtain the correct remainder, which is also annoying to do.
- No reset button. I didn't see a nice way how to clear the output. The previous output is just overwritten by the new output.
## Notes
The CCA design used is by Amino. When posting the schematic using WorldEdit, you should give it one run to make sure everything correctly resetted, and only then start using it.

## Resources
- [SQRT007_32bitsqrtbetter.schem](attachments/SQRT007_32bitsqrtbetter.schem): unknown
