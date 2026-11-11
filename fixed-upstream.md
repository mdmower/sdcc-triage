# Already fixed in trunk

The reported behavior does not occur in trunk. Each entry names the revision that fixed it when that revision was identified.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| [bugs #2221](https://sourceforge.net/p/sdcc/bugs/2221/) | [mov psw is removed from an interrupt routine that selects a register bank and calls a function](tickets/bugs/2221.md) | Close as fixed in r8862 and, for the recurrence of 2018, in r11638. | tested, r17176 |
| [bugs #2287](https://sourceforge.net/p/sdcc/bugs/2287/) | [mcs51 --stack-auto: missing stores to a global in static inline functions that read a va_list](tickets/bugs/2287.md) | Close as fixed, and remove the mcs51 condition in gcc-torture-execute-stdarg-5.c.in. The revision is not identified. | tested, r17176 |
| [bugs #2527](https://sourceforge.net/p/sdcc/bugs/2527/) | [mcs51: stack offsets of spill locations differ between two compilations of one file on Windows 10](tickets/bugs/2527.md) | Close as fixed in r13809, the fix for bug #3505. | tested, r17176 |
| [bugs #2626](https://sourceforge.net/p/sdcc/bugs/2626/) | [sdas ends with a segmentation fault for a macro call with more arguments than parameters](tickets/bugs/2626.md) | Close as fixed in r11332. Consider a q error in place of the internal error for a macro call with too many arguments. | tested, r17176 |
| [bugs #3004](https://sourceforge.net/p/sdcc/bugs/3004/) | [gbz80 -ba: a second .area _DATA line follows the selected data area](tickets/bugs/3004.md) | Close as fixed in r11774. | tested, r17176 |
| [bugs #3077](https://sourceforge.net/p/sdcc/bugs/3077/) | [Names, regression tests, and port coverage of the functions _itoa, _uitoa, _ltoa, and _ultoa](tickets/bugs/3077.md) | Close as fixed in r11731. Decide separately on the pdk patch for __ltoa in comment 23, which is not applied. | tested, r17176 |
| [bugs #3200](https://sourceforge.net/p/sdcc/bugs/3200/) | [DIE references in .debug_info are one byte too high after a source path with a backslash escape](tickets/bugs/3200.md) | Close as fixed in r12964, the fix for bug #3303. r12536 fixed the end-of-siblings markers. | tested, r17176 |
| [bugs #3288](https://sourceforge.net/p/sdcc/bugs/3288/) | [The build prints that makeinfo is missing, and configure does not check for it](tickets/bugs/3288.md) | Close with bug #3192, because on r17176 the build and the installation complete without makeinfo. The revision is not identified. | tested, r17176 |
| [bugs #3303](https://sourceforge.net/p/sdcc/bugs/3303/) | [Backslashes in source paths become control characters in the DWARF sections of an ELF file](tickets/bugs/3303.md) | Close as fixed in r12964. | tested, r17176 |
| [bugs #3337](https://sourceforge.net/p/sdcc/bugs/3337/) | [sdcdb ends with a segmentation fault at break main for a z80 program](tickets/bugs/3337.md) | Close as fixed in r14664, the fix for bug #3529. Close bug #3270 with it, which shows this crash for mcs51. | tested, r17176 |
| [bugs #3489](https://sourceforge.net/p/sdcc/bugs/3489/) | [sdcpp reports a missing C++ compiler for a C file with a .cpp name although -x c is given](tickets/bugs/3489.md) | Close as fixed in r13713, which passes -xc to sdcpp. | tested, r17176 |
| [bugs #3687](https://sourceforge.net/p/sdcc/bugs/3687/) | [mcs51: division and modulo of unsigned char by a constant call __divsint and __modsint](tickets/bugs/3687.md) | Close as fixed in r14650. The longer increments of volatile objects are required, as the fifth comment explains. | tested, r17176 |
| [bugs #3879](https://sourceforge.net/p/sdcc/bugs/3879/) | [Internal error in SDCCopt.c for a member of a union in a struct at a literal address](tickets/bugs/3879.md) | Close as fixed in r15798, the fix for bug #3894. | tested, r17158 |
| [bugs #3886](https://sourceforge.net/p/sdcc/bugs/3886/) | [A compound literal that initializes a struct in a declaration gets no storage](tickets/bugs/3886.md) | Close as fixed in r16747. | tested, r17176 |
