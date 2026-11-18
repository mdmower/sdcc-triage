# Problems without a ticket and without a patch

Problems found during this work that do not have SourceForge tickets and that the fork does not fix. The entries have reproducers. The problems without a ticket that the fork fixes are the `local` entries of the three fix categories.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| local 0015 | [Since r17205, the install rule of device/lib does not copy the mcs51 libraries for --stack-auto](tickets/local/0015.md) | Iterate over ALLPORTS in install and installdirs of device/lib/Makefile.in, or move the stack-auto names to RELPORTS. | tested, r17228 |
| local 0016 | [mcs51 --xstack: the result of a call in r0 is overwritten when one register is restored from the external stack](tickets/local/0016.md) | In unsaveRegisters(), keep r0 in the branch for one register when the result of the call is in r0. | tested, r17228 |
| local 0017 | [mcs51: a C23 function declared (...) reads wrong arguments, and its result in A is lost after a call with more than 3 bytes of arguments](tickets/local/0017.md) | Set FUNC_HASSTACKPARM in processFuncArgs() for a reentrant function declared (...). Make vaargs-c23 execute its assertions. | tested, r17228 |
