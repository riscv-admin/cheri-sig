# CHERI SIG Charter

The CHERI SIG will work on a strategy for adding Capability Hardware Enhanced RISC Instructions (CHERI) to the RISC-V ISA. Enabling a capability-based security model will ensure that RISC-V can provide strong security guarantees as well as mechanisms for compartmentalization that are more scalable than traditional MMU/PMP-based techniques. This SIG will work towards defining a CHERI-enabled instruction set extension, toolchain requirements, programming model and psABI.

## Background:

CHERI is a technology that extends instruction sets with new architectural features (so-called capabilities) to enable fine-grained memory protection and highly scalable software compartmentalization. CHERI was developed at the University of Cambridge and SRI, and it includes [an instantiation for RISC-V (32- and 64-bit) using the custom opcode space](https://github.com/CTSRD-CHERI/cheri-specification).

## Scope:

 * Determine which currently defined architectural CHERI-RISC-V features and instructions are required for a first standardized extension.
 * Scope out the changes to the Qemu, Sail, and LLVM toolchains for this effort.
 * Communicate with other security SIGs and TGs to ensure compatibility.
