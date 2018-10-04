Open-Source RISC-V Architecture IDs
========================================

Every RISC-V hart provides an marchid CSR that encodes its base
microarchitecture.  Any hart may report an architecture ID of 0, indicating
unspecified origin.  Commercial implementations (those with nonzero mvendorid)
may encode any value in marchid with the most-significant bit set, with the
low-order bits formatted in a vendor-specific manner.  Open-source
implementations (which may or may not have a nonzero mvendorid) have the
most-significant bit clear, with a globally unique pattern in the low-order
bits.

This document contains the canonical list of open-source RISC-V implementations
and their architecture IDs.  Open-source project maintainers may make pull
requests against this repository to request the allocation of an architecture
ID.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Project Name | Maintainers                   | Point of Contact                                        | Architecture ID | Project URL
-------------|-------------------------------|---------------------------------------------------------|-----------------|---------------------------------------------------
Rocket       | SiFive, UC Berkeley           | [Andrew Waterman](mailto:andrew@sifive.com), SiFive     |               1 | https://github.com/freechipsproject/rocket-chip
