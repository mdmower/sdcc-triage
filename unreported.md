# Problems without a ticket

Problems found during this work that do not have SourceForge tickets. The entries have reproducers.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| local 0005 | [mcs51 --stack-auto --xstack: stack underflow assertion for calls through a pointer to a function that returns a struct](tickets/local/0005.md) | In genPcall, remove the hidden pointer from the external stack under --xstack, as genCall does. | tested, r17176 |
