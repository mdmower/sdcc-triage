# Problems without a ticket

Problems found during this work that do not have SourceForge tickets. The entries have reproducers.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| local 0002 | [mcs51 small and medium models: compiler crash for global initializers that need address arithmetic at run time](tickets/local/0002.md) | Reject these initializers with error 2 in every model, or give spill locations outside functions a static location. | tested, r17176 |
| local 0004 | [mcs51: compiler crash for functions with a function attribute that return a struct and have a non-struct first parameter](tickets/local/0004.md) | Make the front end and aopArg agree on register parameters of functions that return a struct. | tested, r17176 |
| local 0005 | [mcs51 --stack-auto --xstack: stack underflow assertion for calls through a pointer to a function that returns a struct](tickets/local/0005.md) | In genPcall, remove the hidden pointer from the external stack under --xstack, as genCall does. | tested, r17176 |
| local 0006 | [mcs51: Branching Range Exceeded after peephole rule 257.c replaces sjmp by ljmp between a short jump and its label](tickets/local/0006.md) | Give rule 257.c a condition that keeps the short jumps across its place in range, or remove the rule. | tested, r17176 |
