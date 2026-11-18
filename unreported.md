# Problems without a ticket and without a patch

Problems found during this work that do not have SourceForge tickets and that the fork does not fix. The entries have reproducers. The problems without a ticket that the fork fixes are the `local` entries of the three fix categories.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| local 0015 | [Since r17205, the install rule of device/lib does not copy the mcs51 libraries for --stack-auto](tickets/local/0015.md) | Iterate over ALLPORTS in install and installdirs of device/lib/Makefile.in, or move the stack-auto names to RELPORTS. | tested, r17228 |
