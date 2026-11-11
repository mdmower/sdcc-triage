# Problems without a ticket

Problems found during this work that have no SourceForge ticket. Each entry has a reproducer.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| local 0001 | [Pointers to int that are initialized with wide string literals get bytes of a host address](tickets/local/0001.md) | Fix together with bug #3973, which has the same cause in printIvalPtr. | tested, r17158 |
| local 0002 | [mcs51 small and medium models: compiler crash for global initializers that need address arithmetic at run time](tickets/local/0002.md) | Reject these initializers with error 2 in every model, or give spill locations outside functions a static location. | tested, r17158 |
| local 0003 | [Compound literals under a case label are never initialized](tickets/local/0003.md) | Initialize the object of a compound literal at the place where the literal is evaluated. | tested, r17158 |
| local 0004 | [mcs51: compiler crash for __reentrant functions that return a struct and have a non-struct first parameter](tickets/local/0004.md) | Make the front end and aopArg agree on register parameters of __reentrant functions that return a struct. | tested, r17158 |
| local 0005 | [mcs51 --stack-auto --xstack: stack underflow assertion for calls through a pointer to a function that returns a struct](tickets/local/0005.md) | In genPcall, remove the hidden pointer from the external stack under --xstack, as genCall does. | tested, r17158 |
