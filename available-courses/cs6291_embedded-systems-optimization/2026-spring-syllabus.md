# CS 6291 — Spring 2026 Syllabus

Source: `downloads/CS 6291 2026-1.pdf` (OMSCS sample syllabus, Spring 2026; titled "CS 6291: Embedded Software Optimizations"). The Fall 2024 sample syllabus PDF is byte-identical and is not separately retained. Instructor: Santosh Pande (santosh@cc.gatech.edu).

## Course Objectives

- Understand the tight coupling and synergies between hardware and software in embedded processors, exposed through instruction-set abstractions (DSPs, VLIWs, etc.)
- Understand machine-specific processor features (data paths, register and memory banks) and the machine-specific code optimizations built on them for high performance, compact code, and low energy

## Course Description

Embedded systems — cellular phones, smartphones, tablets, and IoT platforms — have unique processing requirements (real-time responsiveness, high performance at low energy, compact code/data segments, an ever-changing software stack) that have driven ground-up redesign of both hardware and software (ARM, DSPs, network processors; VMs such as Dalvik; operating systems such as Android; new programming models and compiler optimizations). The course takes a holistic view of the embedded-systems stack with a focus on processor architectures, instruction sets, and the associated advanced machine-specific compiler optimizations.

## Prerequisites

An undergraduate computer architecture course and a strong background in C and/or C++ are required.

## Textbooks

1. Fisher, Faraboschi & Young, *Embedded Computing: A VLIW Approach to Architecture, Compilers and Tools* (Morgan Kaufmann, 2004) — available electronically via the Georgia Tech library.
2. Aho, Lam, Sethi & Ullman, *Compilers: Principles, Techniques, and Tools*, 2nd ed. (Addison Wesley, 2006) — recommended reference, not in the GT library electronically.

## Course Outline

**Part I — Embedded Processor Architectures:** instruction-level parallelism (pipelining, RISC vs. CISC, VLIW); instruction-set architecture design; embedded micro-architectures (scratch-pad memory, clustered register files, special arithmetic/addressing, branch speculation and predication).

**Part II — Software Optimizations:** compiler phases; register-allocation foundations (graph-coloring, live-range splitting); register allocation for embedded processors; data layouts; data and code compaction (ARM vs. Thumb); network processors.

## Grading

| Weight | Component |
|---|---|
| 40% | Homework |
| 30% | Projects |
| 30% | Comprehensive Final |

Late penalty: within 48 hours, 15-point penalty; beyond 48 hours, not accepted. GitHub repositories must be kept private. Consult the source PDF for full policies.
