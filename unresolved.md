# Analyzed, not fixed

The problem is reproduced or located, and the fork does not have a patch for it. What is known, and what a fix would involve, is stated in the entry.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| [bugs #3153](https://sourceforge.net/p/sdcc/bugs/3153/) | [Multiple definition of line labels at link time with --debug for static functions defined in a header](tickets/bugs/3153.md) | Keep open for static functions in headers. r12010 fixed the reported case of an inline function without static. | tested, r17176 |
| [bugs #3393](https://sourceforge.net/p/sdcc/bugs/3393/) | [Designated initializer for a member of a nested anonymous union is missing from data images](tickets/bugs/3393.md) | Keep open for the nested-union case of the third comment, or move that case to a new ticket and close this one. | tested, r17176 |
| [bugs #3481](https://sourceforge.net/p/sdcc/bugs/3481/) | [Internal error for a call with arguments to a function declared without a prototype](tickets/bugs/3481.md) | Keep open. Choose between full support, together with feature request #450, and an ordinary error message. | tested, r17158 |
| [bugs #3744](https://sourceforge.net/p/sdcc/bugs/3744/) | [The assemblers of the official Win64 builds crash on source lines that give a q error](tickets/bugs/3744.md) | Keep open. Run the ticket's file with a current official Win64 build, and compare its toolchain with one that builds a working binary. | tested, r17176 |
| [bugs #3920](https://sourceforge.net/p/sdcc/bugs/3920/) | [Ascon tests: four implementations still fail on stm8, and two guards disable cases that pass](tickets/bugs/3920.md) | Keep open. Four implementations still fail on stm8. Recheck the guards for opt32_lowsize on stm8 and for AEAD bi8 on z80. | tested, r17176 |
| [bugs #4034](https://sourceforge.net/p/sdcc/bugs/4034/) | [stm8: SIGSEGV in the DWARF writer for --c1mode with --debug and --out-fmt-elf](tickets/bugs/4034.md) | Keep open. Decide what --debug does in --c1mode, then open the debug file there or add a test to the DWARF writer. | tested, r17158 |
