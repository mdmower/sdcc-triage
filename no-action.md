# No action recommended

The reported behavior is correct, or the request conflicts with the C standard or with documented SDCC behavior. Each entry gives the reason.

| Ticket | Entry | Recommended action | Evidence |
|---|---|---|---|
| [bugs #2536](https://sourceforge.net/p/sdcc/bugs/2536/) | [Error 66 for an array whose size expression (0x1P2 > 10) is zero](tickets/bugs/2536.md) | Close. Keep SKIP_HEXDOUBLE in p99-conformance.c, or change the comparison there to (0x1P2 > 3). | tested, r17176 |
| [bugs #3409](https://sourceforge.net/p/sdcc/bugs/3409/) | [--peep-asm deletes an inline assembler label that only another function references](tickets/bugs/3409.md) | Close. The manual documents both the label restriction and the effect of --peep-asm. | tested, r17176 |
| [bugs #3435](https://sourceforge.net/p/sdcc/bugs/3435/) | [mcs51: a write through a __data pointer with the constant value 0xB0 does not reach P3](tickets/bugs/3435.md) | Close, as the reporter asks in the last comment. Consider a warning for constants above 0x7F cast to __data pointers. | tested, r17176 |
| [bugs #3510](https://sourceforge.net/p/sdcc/bugs/3510/) | [The C version of _modulong does not return when the divisor is zero](tickets/bugs/3510.md) | Close as undefined behavior, or add the zero test of the mcs51 assembly version to the C version. | tested, r17176 |
