# CHERI SIG Charter

The CHERI SIG will work on a strategy for adding Capability Hardware Enhanced RISC Instructions (CHERI) to the RISC-V ISA. Enabling a capability-based security model will ensure that RISC-V can provide strong security guarantees as well as mechanisms for compartmentalization that are more scalable than traditional techniques like PMP (physical memory protection) and MMU (memory management unit). This SIG will work towards defining a CHERI-enabled instruction set extension, toolchain requirements, programming model and psABI (processor-specific application binary interface).

## Background:

CHERI is a technology that extends instruction sets with new architectural features (so-called capabilities) to enable fine-grained memory protection and highly scalable software compartmentalization. CHERI was developed at the University of Cambridge and SRI, and it includes [an instantiation for RISC-V (32- and 64-bit) using the custom opcode space](https://github.com/CTSRD-CHERI/cheri-specification). Microsoft has also announced an IoT-focused adaptation to be published in 2023.

## Scope:

 * Determine which currently defined architectural CHERI-RISC-V features and instructions are required for a first standardized extension.
 * Review changes made to RISC-V ISA baseline since CHERI-RISC-V was developed, to identify gaps where updating may be required -- e.g., around recent work on virtualization and vector extensions.
 * Develop a specification strategy that takes into account both the SRI/Cambridge baseline CHERI-RISC-V and Microsoft's microcontroller-focused variation; this might mean multiple specifications in process concurrently, with a suitable decomposition.
 * Scope out the changes to the Qemu, Sail, and LLVM toolchains for this effort.
 * Communicate with other security SIGs and TGs to ensure compatibility.
