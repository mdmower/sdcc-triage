# Not reproducible

The behavior reported in the ticket could not be reproduced, and a revision with a fix for it was not identified. What was tried is listed in the entry.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| [bugs #2905](https://sourceforge.net/p/sdcc/bugs/2905/) | [mcs51: dead instructions on r5 and r6 in a conditional shift and XOR of a static unsigned char](tickets/bugs/2905.md) | Close as not reproducible on r17176. Review the two peephole patches in the comments as a separate request. | tested, r17176 |
| [bugs #3895](https://sourceforge.net/p/sdcc/bugs/3895/) | [mcs51: internal error in SDCCmem.c for a 128-byte char array with an initializer](tickets/bugs/3895.md) | Close as not reproducible on r17176. local 0002 has other input that fails at the same assertion. | tested, r17176 |
