# Fixes

The cause is identified and the change is confined to it. The patch includes a regression test that fails without the change.

| Ticket | Entry | Recommended action | Evidence | Patch |
|---|---|---|---|---|
| [bugs #2691](https://sourceforge.net/p/sdcc/bugs/2691/) | [Internal error need pointerCode for the address of an element of a nested array of pointers](tickets/bugs/2691.md) | Apply the patch and close. | tested, r17192 | [bugs-2691.patch](patches/bugs-2691.patch) |
| [bugs #3286](https://sourceforge.net/p/sdcc/bugs/3286/) | [mcs51: internal error in getFreePtr for casts of a 64-bit stack parameter with --stack-auto](tickets/bugs/3286.md) | Apply the patch and close. | tested, r17192 | [bugs-3286.patch](patches/bugs-3286.patch) |
| [bugs #3727](https://sourceforge.net/p/sdcc/bugs/3727/) | [GCSE uses the value that a global had before a function call in a loop inside an if](tickets/bugs/3727.md) | Apply the patch and close. | tested, r17192 | [bugs-3727.patch](patches/bugs-3727.patch) |
| [bugs #3847](https://sourceforge.net/p/sdcc/bugs/3847/) | [return of a call's struct value gives an internal error for z80 and writes no result for mcs51](tickets/bugs/3847.md) | Apply the patch and close. | tested, r17192 | [bugs-3847.patch](patches/bugs-3847.patch) |
| [bugs #3849](https://sourceforge.net/p/sdcc/bugs/3849/) | [return of a struct value such as *p crashes the compiler or leaves the caller's object unwritten](tickets/bugs/3849.md) | Apply after the patch for #3847. Check the ticket's example with -msm83, which was not tested, and close. | tested, r17192 | [bugs-3849.patch](patches/bugs-3849.patch) |
| [bugs #3971](https://sourceforge.net/p/sdcc/bugs/3971/) | [SIGSEGV for a string literal plus an offset in the initializer of a static pointer](tickets/bugs/3971.md) | Apply the patch and close. | tested, r17192 | [bugs-3971.patch](patches/bugs-3971.patch) |
| [bugs #4145](https://sourceforge.net/p/sdcc/bugs/4145/) | [SIGSEGV for an expression that combines a run-time value with a constexpr object](tickets/bugs/4145.md) | Apply the patch and close. It has the two guards of the patch attached to the ticket and a third one. | tested, r17192 | [bugs-4145.patch](patches/bugs-4145.patch) |
| [bugs #4228](https://sourceforge.net/p/sdcc/bugs/4228/) | [Internal error for a constexpr or compound literal initializer with _Generic or a constant ?:](tickets/bugs/4228.md) | Apply the patch in place of the one attached to the ticket and close. | tested, r17192 | [bugs-4228.patch](patches/bugs-4228.patch) |
| local 0003 | [Compound literals in function bodies are initialized at the start of their block and not where they are evaluated](tickets/local/0003.md) | Apply the patch. It does not change literals in the initializers of declarations, which Related describes. | tested, r17192 | [local-0003.patch](patches/local-0003.patch) |
| local 0008 | [Arithmetic on the address of an element of a nested array of function pointers steps by a row](tickets/local/0008.md) | Apply the patch. | tested, r17192 | [local-0008.patch](patches/local-0008.patch) |
