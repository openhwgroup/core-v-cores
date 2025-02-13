<img src="https://www.openhwfoundation.org/images/openhw-landscape.png" width="418px" height="103px" /> <img src="https://www.openhwfoundation.org/images/core-v-portrait.png" align="right" width="150px" height="120px"/>

# CORE-V Family of Open-Source RISC-V Cores

CORE-V is a family of permissively licensed, open-source RISC-V cores curated by the OpenHW Foundation ecosystem. Below is the CORE-V Roadmap of Application class and Embedded class cores followed by a short description of each of the cores and links to their respective GitHub repositories.  The overall CORE-V Roadmap as well as core specific features and functionality are driven by [members of the OpenHW Foundation](https://www.openhwgroup.org/#members-partners). Details regarding OpenHW [membership](https://www.openhwgroup.org/membership/#tab-membership) can be found here. The full [OpenHW Project Dashboard](https://github.com/openhwgroup/programs/blob/master/dashboard/Dashboard_SpreadSheetFriendly.md) provides more details about OpenHW projects.

<!-- <img src="https://github.com/openhwgroup/core-v-cores/blob/master/CV-CORES-Roadmap_2023-04-09.png" align="center" /> -->

<!-- <img src="https://github.com/openhwgroup/core-v-cores/blob/master/OpenHW-CoresTimeline-Feb2024.png" align="center" /> -->

<img src="https://github.com/openhwgroup/core-v-cores/blob/master/OpenHW-CoresTimeline-Feb2024-wider.png" align="center" />          


# CORE-V Repositories
## CVA6 Family, 6-Stage Cores configurable as Embedded or Application Class
[CVA6](https://github.com/openhwgroup/cva6), originally known as the PULP Ariane core, is a family of 6-stage, single or dual-issue, in-order cores implementing RV32IMACF_Zicsr_Zifencei or RV64IMACFD_Zicsr_Zifencei (RV64GC) extensions with three privilege levels M, S, U to fully support a Unix-like (Linux, BSD, etc.) operating system. CVA6 has configurable size, separate TLBs, a hardware PTW and branch-prediction (branch target buffer, branch history table and a return address stack).
- [CV32A60AX](https://github.com/openhwgroup/cva6) CV32A60AX is a 32 bit, single-issue application class core supporting RV32IMCA and the [CORE-V eXtension Interface](https://github.com/openhwgroup/core-v-xif) (CV-X-IF).
- [CV32A60X](https://github.com/openhwgroup/cva6) CV32A60X is a 32 bit, single-issue embedded class core supporting RV32IMCA and CV-X-IF support. This device is targeting TRL5 in early 2025.
- [CV64A60AX](https://github.com/openhwgroup/cva6) CV64A60AX is a 64 bit, single-issue application class core supporting RV64IMCADF and CV-X-IF support. This device is targeting TRL4 in 2026.


## CVW (Wally) Family, 5-Stage Cores
[CVW](https://github.com/openhwgroup/cvw) CORE-V Wally is a set of 32-bit and 64-bit RISC-V cores that implement RV32I, RV32E, and RV64I with a 5-stage pipeline,
support for A, C, D, F, and M extensions, and optional caches, branch prediction, virtual memory, AHB, RAMs, and peripherals.
Wally is targeted at Education and will be accompanied by an engineering textbook and course on computer architecture.


## CVE4 Family, 4-Stage Embedded Class Cores
CVE4 is a family of 32-bit, 4-stage in-order cores for embedded platforms that started from the PULP RI5CY core. Single configurations of these cores are maintained on different repositories and specialize in different embedded applications. Below are the members of the CVE4 family.
- [CV32E40Pv1 and CV32E40Pv2](https://github.com/openhwgroup/cv32e40p) Originally known as the PULP RI5CY core, the CORE-V CV32E40P is a 32bit, 4-stage core that implements, RV32IMFC[Xpulp], has an optional 32-bit FPU supporting the F and Zfinx extensions and custom instruction set extensions for DSP operations, including hardware loops, SIMD extensions, bit manipulation and post-increment instructions.  Release 2 supports RV32IMC[F|Zfinx]ZicsrZifenceiZicntr[COREV_PULP][COREV_CLUSTER]. This repository is has been moved (not forked) from the original PULP Platform github repository to its new home at the OpenHW github repository.
- [CV32E40S](https://github.com/openhwgroup/cv32e40s) The CORE-V CV32E40S is a small and efficient, 32-bit, in-order RISC-V core with a 4-stage pipeline that implements the RV32[I|E][M|Zmmul]Zca_Zcb_Zcmp_Zcmt[Zba_Zbb_Zbs|Zba_Zbb_Zbc_Zbs]ZicsrZifenceiXsecure instruction set architecture. The CV32E40S core is aimed at security applications and offers both Machine mode and User mode, an enhanced PMP, and various anti-tampering features.
- [CV32E40X](https://github.com/openhwgroup/cv32e40x) The CORE-V CV32E40X is a small and efficient, 32-bit, in-order RISC-V core with a 4-stage pipeline that implements the RV32[I,E][M|Zmmul][A]Zca_Zcb_Zcmp_Zcmt[Zba_Zbb_Zbs|Zba_Zbb_Zbc_Zbs]ZicntrZihpmZicsrZifencei[X] instruction set architecture. The CV32E40X core is aimed at compute intensive applications and offers a general purpose extension interface [CORE-V-XIF](https://github.com/openhwgroup/core-v-xif) by which custom instructions can be added external to the core.
- [CV32E40PX] The CORE-V CV32E40PX adds RVB, RVP, and RVK support plus CV-X-IF support to the CV32E40PV2.  This device is still in the Project Concept phase.
- [CV32E41P](https://github.com/openhwgroup/cv32e41p) is a small and efficient, 32-bit, in-order RISC-V core with a 4-stage pipeline that implements the RV32IM[F,Zfinx]C[Zce] instruction set architecture, and the Xpulp custom extensions for achieving higher code density, performance, and energy efficiency. Starting as a fork of the CV32E40P core, the E41P then implemented the RISC-V Zfinx and Zce ISA extensions as a prototype to ratify their specification.


## CVE2 Family, 2-Stage Embedded Class Cores
[CVE2](https://github.com/openhwgroup/cve2) is a low-complexity, low-power, 32-bit, in-order RISC-V core with a 2-stage pipeline that implements RV32[E|I][M]C instruction set architecture for achieving high-energy efficiency on control-oriented, computationally limited applications. Starting as a fork of the lowRISC Ibex core, the CVE2 will be pared back to essential components and verified at industrial-grade.


## CVA5 Family, 5-Stage, Application Class Cores for FPGAs
[CVA5](https://github.com/openhwgroup/cva5) The CVA5 is a 32-bit RISC-V processor designed for FPGAs supporting the Multiply/Divide and Atomic extensions (RV32IMA). The processor is written in SystemVerilog and has been designed to be both highly extensible and highly configurable. The CVA5 is derived from the Taiga Project from Simon Fraser University. The pipeline has been designed to support parallel, variable-latency execution units and to readily support the inclusion of new execution units.


# CORE-V Core Names and Releases
Here is an explainer of how [CORE-V Device Names](https://docs.google.com/presentation/d/1MIe9b10-HRglDa67s8oc_2TTYux-WtMY/edit?usp=sharing&ouid=112401338207375688045&rtpof=true&sd=true) are determined.
Any CORE-V core that achieves its target Technical Readiness Level (TRL) spawns a major release (also known as "RTL Freeze") of its host GitHub repository.
A good discussion regarding the rules for creating and updating releases is given [here](https://docs.openhwgroup.org/projects/cv32e40p-user-manual/en/latest/core_versions.html#core-versions-and-rtl-freeze-rules).
At the time of release (freeze), the values `mvendorid`, `marchid` and `mimpid` CSRs are set:
- `mvendorid` is determined by [JEDEC](https://www.jedec.org/).  For OpenHW CORE-V devices the value is `0x602`.
- `marchid` is determined by [RISC-V International](https://github.com/riscv/riscv-isa-manual/blob/main/marchid.md).
A unique `marchid` is provided for each device.
- `mimpid` is determined by OpenHW according to the above rules. The value will be specified in the User Manual.

The Table below summarizes the "ID" values for the CORE-V cores that have been assigned an architecture ID from RVI:

| CORE-V Name | Release | mvendorid  | marchid    | mimpid     | TRL Goal | TRL Achieved | Comment                      |
| ----------- | ------- | ---------- | ---------- | ---------- | -------- | ------------ | ---------------------------- |
| CV32A60X    | TBD     | 0x00000602 | 0x00000003 | 0x00000000 | TRL-5    | Q1, 2025     |                              |
| CV32E40Pv1  | v1.0.0  | 0x00000602 | 0x00000004 | 0x00000000 | TRL-5    | Yes          | F,D,XPULP not verified in v1 |
| CV32E40Pv2  | v1.8.3  | 0x00000602 | 0x00000004 | 0x00000001 | TRL-5    | No [1]       | Target is v2.0.0             |
| CV32E40X    | TBD     | 0x00000602 | 0x00000014 | 0x00000000 | TRL-5    | No [2]       |                              |
| CV32E40S    | TBD     | 0x00000602 | 0x00000015 | 0x00000000 | TRL-5    | No [2]       |                              |
| CV32E41P    | b5d1ba1 | 0x00000602 | 0x0000001C | 0x00000000 | TRL-3    | Archived [3] | "Release" is git hash        |
| CV32E20     | TBD     | 0x00000602 | 0x00000023 | 0x00000000 | TRL-5    | Q4, 2025     |                              |
| CVWally     | TBD     | 0x00000602 | 0x00000024 | 0x00000000 | TRL-5    | Q2, 2025     |                              |

<br><br>
[1] The CV32E40Pv2 is very close to TRL-5 and work is on-going.  Please reach out to a member of OpenHW for more information.
<br>
[2] These devices are mature, but not in active development towards their TRL Goal.
<br>
[3] The CV32E41P was developed as a proof-of-concept.  It is not intended to be used in a Production device.
