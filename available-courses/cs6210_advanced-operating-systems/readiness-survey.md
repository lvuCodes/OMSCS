# CS 6210 — Readiness Resources

Source: `downloads/CS 6210-Diagnostic Preparedness Test.pdf` and `prerequisites-and-concepts-list.pdf` (retained — its programming example references a figure). Both gauge readiness for Advanced Operating Systems.

## Diagnostic Preparedness Test

Self-assessment (answer Yes/No). Largely "no" answers suggest remedial preparation before enrolling.

1. Do you know the conditions under which a process/thread may join and leave the ready queue?
2. Can you name all the steps that happen during a context switch?
3. Can you name at least three types of interprocess communication?
4. Do you know what a data race is in a parallel program?
5. In a preemptive scheduler, do you understand what "preemptive" refers to?
6. Do you understand the difference between round-robin, shortest-job-first, and priority scheduling?
7. Do you know the term for a section of code accessing variables/resources shared between multiple threads?
8. Do you know the necessary and sufficient conditions for deadlock?
9. Do you understand why, when, and how to use mutual exclusion?
10. Can you describe the role of the translation look-aside buffer (TLB) in a virtual memory system?
11. Do you understand the difference between a "segment" and a "page" in a memory hierarchy?
12. Do you know the difference between a "page" and a "frame" in a virtual memory system?
13. Do you know the difference between FIFO, least-recently-used, and least-frequently-used replacement policies?
14. Do you know what it means for a process to "trap" to the kernel?
15. Can you name the mechanism by which asynchronous hardware events notify the CPU/kernel of an event?
16. Can you explain why "ports" are necessary in network communication?
17. Do you know what processor cache (L1, L2) has to do with context switches?
18. Have you written a substantial (not "Hello World") program in C or C++?
19. Have you written a multi-threaded program?
20. Have you written a networked program using a sockets API (Linux/POSIX sockets or winsock)?
21. Have you written a program that handles one or more signals in Linux/POSIX?
22. Do you know how to take timing measurements of a program?

## Prerequisites and Concepts List

### Systems (OS + Networking + Architecture) Concepts

1. Virtual memory — virtual pages vs. physical frames; page tables and TLBs; page replacement (eviction) policies
2. Caches — mechanisms, associativity; replacement policies; coherency mechanisms (update vs. invalidate); L1 & L2 caches and how they attach to cores in multicore architectures
3. SMP vs. NUMA parallel architectures
4. Filesystem and disk basics — data structures, inodes; what a "block device" means and how filesystems and block devices interact
5. Network stack basics — how data flows from/to an app to/from a NIC through protocol-handling layers in the OS
6. Concurrency and synchronization — concurrency vs. parallelism; how the OS switches between processes/kernel threads; how the kernel itself runs (gets control, its stack); scheduling; basic mutual exclusion
7. How a function call/return is implemented in the machine

### Diagnostic Homework on Concepts

Answer in bullet form with figures where appropriate. If most concepts feel foreign, consider remedial action before enrolling.

1. For a processor with virtual memory (virtually indexed, physically tagged cache, TLB, in-memory page table), explain what happens from CPU virtual-address generation to the referenced memory contents being available.
2. Distinguish between segmentation and paging.
3. Explain all actions from a page fault to resumed execution (assume the only runnable process).
4. Explain: working set of a process, thrashing, paging daemon, swapper, loader, linker.
5. Explain page coloring and its use in memory management.
6. Explain the costs of a process context switch.
7. Explain the functionality of the different layers in an OS network protocol stack (e.g., Linux).

### C Programming Skills

1. Pointers — general use, `*` and `&` operators, "box & arrow" reasoning, struct-ptr vs. struct assignment
2. Function pointers
3. Dynamic memory management (`malloc` & `free`)
4. Process memory layout — stack, heap, global data, code; pointers to memory in different segments
5. Data representation — everything is just bits
6. Casting — especially non-obvious casts (ptr ↔ int, anything ↔ `void*`)
7. Compiling & linking — header files, libraries (`.a`), declarations vs. definitions
8. Segfaults — why they happen and how to debug them
9. Race conditions & bugs

### Example Programming Project

A multithreaded producer-consumer program using the pthreads library, modeled on a video-based surveillance application (digitizer → tracker → alarm). The digitizer converts video into frames of pixels, the tracker analyzes each frame for content needing flagging, and the alarm takes control action. Assume the three components are available as callable functions; implement the producer-consumer functionality between them. (See the retained PDF for the accompanying figure.)
