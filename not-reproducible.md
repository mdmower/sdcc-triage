# Not reproducible

The reported behavior could not be reproduced, and no revision that fixed it was identified. Each entry lists what was tried.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| [bugs #2287](https://sourceforge.net/p/sdcc/bugs/2287/) | [mcs51 --stack-auto: missing stores to a global in static inline functions that read a va_list](tickets/bugs/2287.md) | Remove the mcs51 condition in gcc-torture-execute-stdarg-5.c.in, run the test, and close the ticket if it passes. | tested, r17158 |
| [bugs #3703](https://sourceforge.net/p/sdcc/bugs/3703/) | [sdas8051: wrong location counter at .ORG after branches to numeric addresses](tickets/bugs/3703.md) | Close as not reproducible on r17158, or ask the reporter to retest with a current build. | tested, r17158 |
| [bugs #3895](https://sourceforge.net/p/sdcc/bugs/3895/) | [mcs51: internal error in SDCCmem.c for a 128-byte char array with an initializer](tickets/bugs/3895.md) | Close as not reproducible on r17158. local 0002 has other input that fails at the same assertion. | tested, r17158 |
