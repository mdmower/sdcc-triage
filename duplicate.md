# Duplicates

The same problem is already reported in another ticket.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| [bugs #3527](https://sourceforge.net/p/sdcc/bugs/3527/) | [sdas evaluates constants as 24-bit signed values, so a shift by 24 gives 0x00 or 0xFF](tickets/bugs/3527.md) | Close as a duplicate of bug #4070. Add the two constants of this ticket to the test for that fix. | tested, r17176 |
| [bugs #3763](https://sourceforge.net/p/sdcc/bugs/3763/) | [sdas8051.exe of the 4.4.0 Win64 release crashes on a source line with a syntax error](tickets/bugs/3763.md) | Close as a duplicate of bug #3744. Examine the longjmp call of the q error path in the Win64 release build. | tested, r17176 |
