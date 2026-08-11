# 32 bit cube root extractor
<img alt="2026-08-12_01.09.49.png" src="images/2026-08-12_01.09.49.png?raw=1" height="300px">

**Authors:** *mcdnldsmngr*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1536878871755100323)

Device computes C = floor(cuberoot(A)) and remainder R such that A = C^3 + R. It includes a “Clock” button to start computation and a “Reset” button in the back to clear outputs.
## Input
Takes in a 32 Bit number A.
## Output
Returns C = floor(cuberoot(A)) and the remainder R, i.e. A = C^3 + R.
## Speed
Does 11 iterations, with one iteration needing 28rt (i.e. 2.8 sec). In total, it takes a little over 30 seconds.
## Notes
Uses a CCA design by Amino. Algorithm: r ← (r << 3) | next_3_bits; trial ← S + 6p + 1; if r ≥ trial then r ← r − trial; S ← (S << 2) + 48p + 12; p ← 2p + 1; else S ← S << 2; p ← 2p.

## Resources
- [OTHERARITH009_32bitcbrt.schem](attachments/OTHERARITH009_32bitcbrt.schem): unknown
