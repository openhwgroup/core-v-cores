# core-v-cores
CORE-V Family of Open Source RISC-V Cores

Here are the links to the OpenHW Group CORE-V Family of RISC-V cores:

[CV32E40P](https://github.com/openhwgroup/cv32e40p) Originally known as the PULP RI5CY core, the CORE-V CV32E40P is a 32bit, 4-stage core that implements, RV32IMFC[Xpulp], has an optional 32-bit FPU supporting the F extension and instruction set extensions for DSP operations, including hardware loops, SIMD extensions, bit manipulation and post-increment instructions.  This repository is has been moved (not forked) from the original PULP Platform github repository to its new home at the OpenHW Group github repository.

[CVA6](https://github.com/openhwgroup/cva6) Originally known as the PULP Ariane core, the CORE-V CVA6 6-stage, single issue, in-order core implementing RV32GC or RV64GC extensions with three privilege levels M, S, U to fully support a Unix-like (Linux, BSD, etc.) operating system. It has configurable size, separate TLBs, a hardware PTW and branch-prediction (branch target buffer, branch history table and a return address stack).

[CV32E40X](https://github.com/openhwgroup/cv32e40x) The CORE-V CV32E40X is a small and efficient, 32-bit, in-order RISC-V core with a 4-stage pipeline that implements the RV32IM[A]C[B][P]XZce_Zicount_Zicsr_Zifencei instruction set architecture. The CV32E40X core is aimed at compute intensive applications and offers a general purpose extension interface by which custom instructions can be added external to the core.

[CV32E40S](https://github.com/openhwgroup/cv32e40s) The CORE-V CV32E40S is a small and efficient, 32-bit, in-order RISC-V core with a 4-stage pipeline that implements the RV32IMCXsecureZce_Zicsr_Zifencei instruction set architecture. The CV32E40S core is aimed at security applications and offers both Machine mode and User mode, an enhanced PMP, as well as various anti-tampering features.
