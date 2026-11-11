# Analyzed, not fixed

The problem is reproduced or located, and no patch is offered. Each entry says what is known and what a fix would involve.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| [bugs #3481](https://sourceforge.net/p/sdcc/bugs/3481/) | [Internal error for a call with arguments to a function declared without a prototype](tickets/bugs/3481.md) | Keep open. Choose between full support, together with feature request #450, and an ordinary error message. | tested, r17158 |
| [bugs #3973](https://sourceforge.net/p/sdcc/bugs/3973/) | [String literals that initialize void pointers or integers are emitted as bytes of a host address](tickets/bugs/3973.md) | Keep open. The cause is in printIvalPtr and printIvalType in src/SDCCglue.c. No patch is offered. | tested, r17158 |
| [bugs #4034](https://sourceforge.net/p/sdcc/bugs/4034/) | [stm8: SIGSEGV in the DWARF writer for --c1mode with --debug and --out-fmt-elf](tickets/bugs/4034.md) | Keep open. Decide what --debug does in --c1mode, then open the debug file there or add a test to the DWARF writer. | tested, r17158 |
| [bugs #4070](https://sourceforge.net/p/sdcc/bugs/4070/) | [sdas8051 assembles the address of the fourth byte of an __sfr32 as 0xFF](tickets/bugs/4070.md) | Choose between the valmasks patch in the ticket and the upstream asxxxx design. Add a test that reads each byte through an __sfr. | tested, r17158 |
