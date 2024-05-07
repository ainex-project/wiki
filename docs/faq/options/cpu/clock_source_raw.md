<!--- This file is a snippet --->
Use the `RDTSC` instruction as the time source.

**Host CPU must support invariant TSC.**

| **clock_source_raw**                                      | **bool** |
|:----------------------------------------------------------|:--------:|
| Gets the guest time using the system clock. (**default**) |  false   |
| Gets the guest time using the `RDTSC` instruction.        |   true   |
