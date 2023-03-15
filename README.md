<img src="https://www.openhwgroup.org/images/openhw-landscape.png" width="418px" height="103px" /> <img src="https://www.openhwgroup.org/images/core-v-portrait.png" align="right" width="150px" height="120px"/>

# CORE-V Family of Open-Source RISC-V Cores

CORE-V is a family of permissively licensed, open-source RISC-V cores currated by the OpenHW Group ecosystem. Below is the CORE-V Roadmap of Application class and Embedded class cores followed by a short description of each of the cores and links to their respective GitHub repositories.  The overall CORE-V Roadmap as well as core specific features and functionality are driven by [members of the OpenHW Group](https://www.openhwgroup.org/#members-partners). Details regarding [OpenHW Group membership can be found here.](https://www.openhwgroup.org/membership/#tab-membership). The full [OpenHW Project Dashboard](https://github.com/openhwgroup/programs/blob/master/dashboard/Dashboard_SpreadSheetFriendly.md) provides more details about OpenHW projects.

<img src="https://github.com/openhwgroup/core-v-cores/blob/master/CV-CORES-Roadmap_2023-03-14.png" align="center" />


# CORE-V Application Class, 5/6-Stage Cores

[CVA6](https://github.com/openhwgroup/cva6) Originally known as the PULP Ariane core, the CORE-V CVA6 6-stage, single issue, in-order core implementing RV32GC or RV64GC extensions with three privilege levels M, S, U to fully support a Unix-like (Linux, BSD, etc.) operating system. It has configurable size, separate TLBs, a hardware PTW and branch-prediction (branch target buffer, branch history table and a return address stack).

[CVA5](https://github.com/openhwgroup/cva5) The CVA5 is a 32-bit RISC-V processor designed for FPGAs supporting the Multiply/Divide and Atomic extensions (RV32IMA). The processor is written in SystemVerilog and has been designed to be both highly extensible and highly configurable. The CVA5 is derived from the Taiga Project from Simon Fraser University. The pipeline has been designed to support parallel, variable-latency execution units and to readily support the inclusion of new execution units.

[CORE-V Wally](https://github.com/openhwgroup/cvw) CORE-V Wally is a set of 32-bit and 64-bit RISC-V cores that implement RV32I, RV32E, and RV64I with a 5-stage pipeline, support for A, C, D, F, and M extensions, and optional caches, branch
prediction, virtual memory, AHB, RAMs, and peripherals. Wally is targeted at Education and will be accompanied by an engineering textbook and course on computer architecture.


# CORE-V Embedded Class, 4-Stage Cores

CVE4 is a family of cores for embedded platforms that started from the PULP RI5CY core. These cores are 32bit, 4-stage in-order cores. Single configurations of these cores are maintained on different repositories and specialize in different embedded applications. Please find below the members of the CVE4 family.

- [CV32E40P](https://github.com/openhwgroup/cv32e40p) Originally known as the PULP RI5CY core, the CORE-V CV32E40P is a 32bit, 4-stage core that implements, RV32IMFC[Xpulp], has an optional 32-bit FPU supporting the F and Zfinx extensions and custom instruction set extensions for DSP operations, including hardware loops, SIMD extensions, bit manipulation and post-increment instructions.  This repository is has been moved (not forked) from the original PULP Platform github repository to its new home at the OpenHW Group github repository.

- [CV32E40X](https://github.com/openhwgroup/cv32e40x) The CORE-V CV32E40X is a small and efficient, 32-bit, in-order RISC-V core with a 4-stage pipeline that implements the RV32[I,E][M|Zmmul][A]Zca_Zcb_Zcmp_Zcmt[Zba_Zbb_Zbs|Zba_Zbb_Zbc_Zbs]ZicntrZihpmZicsrZifencei[X] instruction set architecture. The CV32E40X core is aimed at compute intensive applications and offers a general purpose extension interface [CORE-V-XIF](https://github.com/openhwgroup/core-v-xif) by which custom instructions can be added external to the core.

- [CV32E40S](https://github.com/openhwgroup/cv32e40s) The CORE-V CV32E40S is a small and efficient, 32-bit, in-order RISC-V core with a 4-stage pipeline that implements the RV32[I|E][M|Zmmul]Zca_Zcb_Zcmp_Zcmt[Zba_Zbb_Zbs|Zba_Zbb_Zbc_Zbs]ZicsrZifenceiXsecure instruction set architecture. The CV32E40S core is aimed at security applications and offers both Machine mode and User mode, an enhanced PMP, and various anti-tampering features.

- [CV32E41P](https://github.com/openhwgroup/cv32e41p) is a small and efficient, 32-bit, in-order RISC-V core with a 4-stage pipeline that implements the RV32IM[F,Zfinx]C[Zce] instruction set architecture, and the Xpulp custom extensions for achieving higher code density, performance, and energy efficiency. Starting as a fork of the CV32E40P core, the E41P then implemented the official RISC-V Zfinx and Zce ISA extensions.

# CORE-V Embedded Class, 2-Stage Core

[CVE2](https://github.com/openhwgroup/cve2) is a low-complexity, low-power, 32-bit, in-order RISC-V core with a 2-stage pipeline that implements RV32[E|I][M]C instruction set architecture for achieving high-energy efficiency on control-oriented, computationally limited applications. Starting as a fork of the lowRISC Ibex core, the CVE2 will be pared back to essential components and verified at industrial-grade.
