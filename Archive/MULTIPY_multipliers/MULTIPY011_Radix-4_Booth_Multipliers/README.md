# Radix-4 Booth Multipliers
<img alt="2026-08-19_00.05.24.png" src="images/2026-08-19_00.05.24.png?raw=1" height="300px">

**Authors:** *mcdnldsmngr*

**Endorsed by:** *Mixel*

**Tags:** *Tested & Functional*

**Original post:** [View on Discord](https://discord.com/channels/1361854816837435433/1539410992054796330)

Multiplies two unsigned 8/16/32-bit numbers to produce an unsigned product using a radix-4 Booth algorithm and specific CSA/CCA looping approaches.
## Input
Two unsigned 8 / 16 / 32 bit numbers
## Output
Unsigned 16 / 32 / 64 bit product
## Speed
Processes two bits of A every 3rd, so does 4 / 8 / 16 iterations with one iteration being 3rd. The 32 bit multiplier shows the result less than 10 seconds after pressing the "Start" button (as far as I am aware).
## Considerations
- Uses 3t looping CSA shown in Bennyscube video and 3t CCA by Amino.
- Uses the Radix-4 Booth algorithm which essentially also works for signed numbers in twos complement, but this would require additional logic afaik

## Resources
- [MULTIPY011_r4bmult.schem](attachments/MULTIPY011_r4bmult.schem): unknown
