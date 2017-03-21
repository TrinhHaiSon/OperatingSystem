## Memory management

### 1. Basic hardware
Main memory and registers built into the processor itself are the only storage that the CPU can access directly. There are machine intructions that take memory address as arguments but none that take dish addresses. Therefore, any instructions in execution and any date being used must be in one of the direct-access storage devices. If the data are not in memory, they must be moved therefore CPU can operate on them.  
We must ensure the correct operation has to protect the operating system from access by user processes, in addition, to protect user processes from one another. This protection must be protected by hardware. In this section we outline one possible implementation.  
Each process has its own separate memory space. To do that we need the ability to determine the length of legal adrresses that the process may access and to ensure that the process can access only the legal addresses. We can provide this protection by using two registers, usually a base and a limit. The base register hold the smallest legal physical address; the limit register specify the range.
