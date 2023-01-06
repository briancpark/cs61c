# CS 61C

CS 61C is Great Ideas in Computer Architecture (Machine Structures) at UC Berkeley. I took this offering in Fall 2020 under Dan Garcia and Borivoje Nikolic. This repo contains my development setup and notes.

There is no source code here and the submodules are made private. Please DO NOT contact me for source code.

## Development Setup

Labs were done with a variety of setups that should work after we install the required tools for projects.

Project 1 was done in C. `gcc` and `clang` compilers should work, since the codebase is C99 compliant.

Project 2 was done in RISC-V assembly. But it uses Venus, a RISC-V simulator, to run the code. The simulator is written in Java, so you need to have Java installed. Unittests are written in Python, so that needs to be installed as well. After that, code should be runnable and reproducable.

Project 3 was done in Logisim, a digital logic simulator. You can download it [here](http://www.cburch.com/logisim/). This also requires Java to be installed.

Project 4 was done in C and Python. Not only `gcc` is required, but specifically Python 3.6 is required to properly build the library. Note that hardware supported with AVX2 is required for the C code to compile and run. The reference solution shared library file is included with the repo and requires Linux.

Since Project 4 was a performance programming project, it requires the same CPU in order to reproduce the results. The CPU specs we used are as follows:

```
Architecture:          x86_64
CPU op-mode(s):        32-bit, 64-bit
Byte Order:            Little Endian
CPU(s):                8
On-line CPU(s) list:   0-7
Thread(s) per core:    2
Core(s) per socket:    4
Socket(s):             1
NUMA node(s):          1
Vendor ID:             GenuineIntel
CPU family:            6
Model:                 60
Model name:            Intel(R) Core(TM) i7-4770 CPU @ 3.40GHz
Stepping:              3
CPU MHz:               3400.000
CPU max MHz:           3900.0000
CPU min MHz:           800.0000
BogoMIPS:              6784.75
Virtualization:        VT-x
L1d cache:             32K
L1i cache:             32K
L2 cache:              256K
L3 cache:              8192K
NUMA node0 CPU(s):     0-7
Flags:                 fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc aperfmperf eagerfpu pni pclmulqdq dtes64 monitor ds_cpl vmx smx est tm2 ssse3 sdbg fma cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand lahf_lm abm epb invpcid_single kaiser tpr_shadow vnmi flexpriority ept vpid fsgsbase tsc_adjust bmi1 avx2 smep bmi2 erms invpcid xsaveopt dtherm ida arat pln pts
```
