# Duplicates

The same problem is already reported in another ticket.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| [bugs #3527](https://sourceforge.net/p/sdcc/bugs/3527/) | [sdas evaluates constants as 24-bit signed values, so a shift by 24 gives 0x00 or 0xFF](tickets/bugs/3527.md) | Close as a duplicate of bug #4070 when the fix for that ticket covers the pdk assemblers. The patch for #4070 in this report changes sdas8051 alone. | tested, r17176 |
| [bugs #3763](https://sourceforge.net/p/sdcc/bugs/3763/) | [sdas8051.exe of the 4.4.0 Win64 release crashes on a source line with a syntax error](tickets/bugs/3763.md) | Close as a duplicate of bug #3744. Examine the longjmp call of the q error path in the Win64 release build. | tested, r17176 |
| [bugs #4250](https://sourceforge.net/p/sdcc/bugs/4250/) | [return of a struct member such as w.in gives an internal error for stm8 and z80 and wrong bytes for mcs51](tickets/bugs/4250.md) | Close as a duplicate of bug #3849. The patch for #3849 in this report is for the statements of this ticket. | tested, r17193 |
| [patches #516](https://sourceforge.net/p/sdcc/patches/516/) | [Patch for bug #4054 that changes geniCodeSEParms for struct arguments of the form *p](tickets/patches/516.md) | Close together with bug #4054 when the patch of that entry is applied. This patch was read and was not built. | read, r17193 |
