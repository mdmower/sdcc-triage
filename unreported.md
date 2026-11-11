# Problems without a ticket

Problems found during this work that do not have SourceForge tickets. The entries have reproducers.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| local 0001 | [Pointers to int that are initialized with wide string literals get bytes of a host address](tickets/local/0001.md) | Fix together with bug #3973, which has the same cause in printIvalPtr. | tested, r17176 |
| local 0002 | [mcs51 small and medium models: compiler crash for global initializers that need address arithmetic at run time](tickets/local/0002.md) | Reject these initializers with error 2 in every model, or give spill locations outside functions a static location. | tested, r17176 |
| local 0003 | [Compound literals in function bodies are initialized once at the start of the enclosing block](tickets/local/0003.md) | Initialize the object of a compound literal at the place where the literal is evaluated. | tested, r17176 |
| local 0004 | [mcs51: compiler crash for functions with a function attribute that return a struct and have a non-struct first parameter](tickets/local/0004.md) | Make the front end and aopArg agree on register parameters of functions that return a struct. | tested, r17176 |
| local 0005 | [mcs51 --stack-auto --xstack: stack underflow assertion for calls through a pointer to a function that returns a struct](tickets/local/0005.md) | In genPcall, remove the hidden pointer from the external stack under --xstack, as genCall does. | tested, r17176 |
| local 0006 | [mcs51: Branching Range Exceeded after peephole rule 257.c replaces sjmp by ljmp between a short jump and its label](tickets/local/0006.md) | Give rule 257.c a condition that keeps the short jumps across its place in range, or remove the rule. | tested, r17176 |
| local 0007 | [mcs51: reads such as *a[1][1] through an element of a nested array of pointers in data memory first store the pointer through itself](tickets/local/0007.md) | Do not let geniCodeDerefPtr set isaddr on the result operand of the iCode that geniCodeRValue has just emitted. | tested, r17176 |
| local 0008 | [Arithmetic on the address of an element of a nested array of function pointers steps by a row](tickets/local/0008.md) | In geniCodeArray and geniCodeAddressOf, give &fp[i][j] the type pointer to element when the elements are function pointers. | tested, r17176 |
| local 0010 | [sdld: a PC-relative byte after another byte with a relocation on the same T line gets a displacement that is 2 too low](tickets/local/0010.md) | In relr3, add 2 to rtofst after each byte relocation with R_BYT3. The change was not built or tested. | tested, r17176 |
