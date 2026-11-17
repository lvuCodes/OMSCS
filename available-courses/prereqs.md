# Course Prerequisites and Recommended Background

Prerequisites and recommended background for **all OMSCS-applicable courses** — the 75 courses on the official [OMSCS current-courses listing](https://omscs.gatech.edu/current-courses), not only the Fall 2026 registration set.

OMSCS system-enforces almost none of these; they are self-assessed expectations. Each entry is sourced from the course's **official syllabus** `Prerequisites` section where one exists (the most authoritative source), falling back to the course-page "Before Taking This Class" section otherwise.

## Reading the Tables

| Element | Meaning |
|---|---|
| **Course Prereq** | Required prior **GT courses** (or named course-equivalent coursework). |
| **Rec. Course Prereq** | Prior GT courses that are recommended, not required. |
| **Knowledge (High)** | Required knowledge, skills, and math background. |
| **Knowledge (Low)** | Recommended knowledge/skills — improve grade or reduce ramp-up, not gating. |
| **Exceptions** | Equivalency allowances, instructor-consent paths, readiness seminars, certification/account needs, audit restrictions, "no formal prerequisites" notes. |
| **Source** | Origin of the row. **⏳ = needs fresh re-pull** (course page or pre-2025 syllabus, not a current 2025–26 syllabus). |
| 🔒 | Marks a **formally enforced enrollment gate** — a specific grade minimum, instructor consent, or required completion (vs. a self-assessed expectation). |
| **Bold code** | A course code in a prereq column, for quick scanning. `—` = none stated. |

## CS Core

| Course | Course Prereq | Rec. Course Prereq | Knowledge (High) | Knowledge (Low) | Exceptions | Source |
|---|---|---|---|---|---|---|
| [CS 6035 — Intro to Information Security](cs6035_introduction-to-information-security/readiness-survey.md) | — | — | CS fundamentals; C, Python, Java, SQL; data structures, algorithms, complexity; Linux CLI; VirtualBox | Discrete math, modular arithmetic; assembly, `gdb`; Wireshark; NumPy/pandas; web-sec (XSS/CSRF, SQLi) | — | Course page ⏳ |
| [CS 6150 — Computing for Good](cs6150_computing-for-good/readiness-survey.md) | Grad coursework in ≥2 of 7 areas (databases, networking, web dev, global health, etc.) | — | — | — | — | Syllabus 2024 ⏳ |
| [CS 6200 — Intro to Operating Systems](cs6200_introduction-to-operating-systems/readiness-survey.md) | — | Undergrad OS course | C, C++; computer systems/architecture; OS abstractions (process, thread, page table, scheduling) | Linux CLI; Vagrant/VirtualBox; Makefiles; GDB | — | Course page ⏳ |
| [CS 6210 — Advanced Operating Systems](cs6210_advanced-operating-systems/readiness-survey.md) | — | Undergrad OS course | Substantial C/C++; multithreading; OS internals (VM, scheduling, sync, deadlock); pointers, dynamic memory | Sockets/network programming; signals | — | Course page ⏳ |
| [CS 6211 — System Design for Cloud Computing](cs6211_system-design-for-cloud-computing/readiness-survey.md) | 🔒 **CS 4210/6210** | — | — | — | Instructor consent for equivalent; course page wants grade A / high B | Syllabus (current) |
| [CS 6238 — Secure Computer Systems](cs6238_secure-computer-systems/readiness-survey.md) | Undergrad OS (**CS 3210**) | — | C; Python; Linux, system calls | — | CS 3210 "or equivalent" | Course page ⏳ |
| [CS 6250 — Computer Networks](cs6250_computer-networks/readiness-survey.md) | — | Prior networking course | Intermediate Python; networking basics (IP, subnets, TCP/UDP, OSI, handshakes, HTTP) | VMs | — | Syllabus 2024 ⏳ |
| [CS 6260 — Applied Cryptography](cs6260_applied-cryptography/readiness-survey.md) | — | — | Math maturity (proofs); discrete math; algorithms & complexity; basic probability | — | No crypto needed (number theory taught) | Syllabus 2024 ⏳ |
| [CS 6261 — Security Ops & Incident Response](cs6261_security-operations-and-incident-response/readiness-survey.md) | — | — | System logs & log-analysis (Splunk); systems & networks | — | — | Syllabus 2025-spring |
| [CS 6262 — Network Security](cs6262_network-security/readiness-survey.md) | — | **CS 6035** | Info-security basics | Web dev (JS/DOM, HTML, CSS, DevTools); XSS, SOP; Python; disassembly; network protocols; Wireshark, Snort | Weaker programmers advised to take CS 6035 first; minimal overlap | Syllabus 2026-spring |
| [CS 6263 — Intro to Cyber-Physical Systems Security](cs6263_intro-to-cyber-physical-systems-security/readiness-survey.md) | A networking class; an info-security class | — | Python | — | — | Syllabus 2026-summer |
| [CS 6264 — Info Security Lab: System & Network Defenses](cs6264_information-security-lab-system-and-network-defenses/readiness-survey.md) | Intro info-security course | Network-security course (**CS 6262**) | C, Java, or similar | — | Small overlap w/ CS 6035 / 6262 | Syllabus 2025-fall |
| [CS 6265 — Information Security Lab](cs6265_information-security-lab/readiness-survey.md) | OS (**CS 3210**) | — | — | — | CS 3210 "equivalent"; needs internet, Adobe Acrobat | Syllabus 2026-spring |
| [CS 6271 — Cybersecurity of Drones](cs6271_cybersecurity-of-drones/readiness-survey.md) | — | — | Basic C/C++; computer architecture & embedded systems; cybersecurity fundamentals | Control systems, signal processing; OS, reverse engineering | — | Syllabus 2026-summer |
| [CS 6290 — High Performance Computer Architecture](cs6290_high-performance-computer-architecture/readiness-survey.md) | — | Undergrad computer organization | — | ISAs & pipelining; C/C++, Linux | — | Course page ⏳ |
| [CS 6291 — Embedded Systems Optimization](cs6291_embedded-systems-optimization/readiness-survey.md) | Undergrad computer architecture | — | Strong C/C++ | Python (basic–intermediate); git | — | Syllabus 2026-spring |
| [CS 6300 — Software Development Process](cs6300_software-development-process/readiness-survey.md) | A prior SWE course | — | SWE concepts (requirements, design, testing); Java | Learning new tools; remote-team availability | Industry SWE experience substitutes; other OO lang may suffice | Syllabus 2026-spring |
| [CS 6310 — Software Architecture & Design](cs6310_software-architecture-and-design/readiness-survey.md) | 🔒 **CS 6300** (grade D+) | — | Solid programming; basic Java (control structures, file I/O); a defined design process | — | Industry experience may substitute; can learn Java from another lang | Syllabus 2026-summer |
| [CS 6340 — Software Analysis](cs6340_software-analysis/readiness-survey.md) | — | — | C-family fluency (C/C++/Java/C#; labs C++); CS & math basics; UNIX tooling | — | See Readiness Assessment | Syllabus 2025-spring |
| [CS 6400 — Database Systems Concepts & Design](cs6400_database-systems-concepts-and-design/readiness-survey.md) | — | — | A scripting/programming lang (PHP/Python/Java) | SWE, Git; sysadmin willingness; remote teamwork | — | Syllabus 2025-spring |
| [CS 6422 — Database System Implementation](cs6422_database-system-implementation/readiness-survey.md) | **CS 1332**, **CS 2200** | **CS 3210** (OS), **CS 4400** (databases) | C++; systems programming & SWE foundation | — | — | Syllabus 2026-spring |
| [CS 6435 — Digital Health Equity](cs6435_digital-health-equity/readiness-survey.md) | — | — | — | — | — | Course page |
| [CS 6440 — Intro to Health Informatics](cs6440_intro-to-health-informatics/readiness-survey.md) | — | — | CS basics; a modern lang (Java/Python/JS/TS) | Web-app deployment | No health-informatics knowledge needed | Course page ⏳ |
| [CS 6457 — Video Game Design](cs6457_video-game-design/readiness-survey.md) | — | — | C# | Java/strongly-typed OO; linear algebra & graphics basics (affine transforms, quaternions, 3D projection, scene graphs, Phong) | Unity not assumed | Syllabus 2022 ⏳ |
| [CS 6460 — Educational Technology](cs6460_educational-technology/readiness-survey.md) | 🔒 OMSCS foundational-area requirement | — | — | Essays, projects, open-ended learning | — | Course page ⏳ |
| [CS 6475 — Computational Photography](cs6475_computational-photography/readiness-survey.md) | — | — | Programming (Python); college math (matrices, vectors, calculus); physics (vectors, optics); probability; camera basics | OpenCV, NumPy | — | Course page ⏳ |
| [CS 6476 — Computer Vision](cs6476_computer-vision/readiness-survey.md) | — | — | Python; linear algebra; vector calculus; probability | Image-processing basics | — | Course page ⏳ |
| [CS 6491 — Foundations of Computer Graphics](cs6491_foundations-of-computer-graphics/readiness-survey.md) | — | — | — | — | Graphics fundamentals reviewed in course | Course page |
| [CS 6515 — Intro to Graduate Algorithms](cs6515_intro-to-graduate-algorithms/readiness-survey.md) | — | — | Undergrad algorithms (DP, divide & conquer, graph algorithms, recurrences, asymptotics); discrete math | — | CS 8001 OLP seminar fulfills the prereq | Course page ⏳ |
| [CS 6601 — Artificial Intelligence](cs6601_artificial-intelligence/readiness-survey.md) | — | — | Python (+ notebooks); algorithms & data structures; linear algebra, probability, calculus; ~9 hrs/wk | Prior intensive programming courses | — | Course page ⏳ |
| [CS 6603 — AI, Ethics, and Society](cs6603_ai-ethics-and-society/readiness-survey.md) | — | — | Prior programming; Python, Jupyter | — | Social-media presence for some Module 1 work | Course page ⏳ |
| [CS 6675 — Advanced Internet Systems & Applications](cs6675_advanced-internet-systems-and-applications/readiness-survey.md) | — | — | Computing & networking fundamentals | — | — | Course page ⏳ |
| [CS 6747 — Advanced Malware Analysis](cs6747_advanced-malware-analysis/readiness-survey.md) | — | — | — | — | — | Course page |
| [CS 6750 — Human-Computer Interaction](cs6750_human-computer-interaction/readiness-survey.md) | — | — | — | — | No significant prerequisites | Course page |
| [CS 6795 — Intro to Cognitive Science](cs6795_introduction-to-cognitive-science/readiness-survey.md) | — | — | — | — | No significant prerequisites | Course page |
| [CS 7210 — Distributed Computing](cs7210_distributed-computing/readiness-survey.md) | — | **CS 6200**, **CS 6210**, or **CS 6250** | Graduate systems/networking understanding | — | None enforced | Syllabus 2025-fall |
| [CS 7240 — Modern Internet Research Methods](cs7240_modern-internet-research-methods/readiness-survey.md) | — | — | Open-ended problems; peer feedback | Coding (systems / ML-AI / viz / algo projects) | Prereqs depend on project | Syllabus 2026-spring |
| [CS 7280 — Network Science](cs7280_network-science/readiness-survey.md) | — | — | Undergrad calculus, probability, linear algebra, programming | — | No Audit | Course page ⏳ |
| [CS 7295 — GPU Hardware and Software](cs7295_gpu-hardware-and-software/readiness-survey.md) | — | **CS 6200**, **CS 6290**, **CSE 6220**, or **CS 6340** (by project) | C/C++, Python; Linux CLI; computer organization (ISAs, pipelining) | — | Prior CUDA not needed | Syllabus 2026-spring |
| [CS 7400 — Intro to Quantum Computing](cs7400_intro-to-quantum-computing/readiness-survey.md) | — | — | — | — | Linear algebra reviewed in course | Course page ⏳ |
| [CS 7470 — Mobile & Ubiquitous Computing](cs7470_mobile-and-ubiquitous-computing/readiness-survey.md) | 🔒 **CS 2110** or **CS 2261** (grade C) | — | — | Web/version control; Python/R/Matlab | 🔒 CITI cert for human-participant projects | Syllabus 2024 ⏳ |
| [CS 7496 — Computer Animation](cs7496_computer-animation/readiness-survey.md) | — | **CS 3451** (graphics) | Linear algebra, vector calculus; OOP | Python | — | Syllabus 2026-spring |
| [CS 7632 — Game AI](cs7632_game-ai/readiness-survey.md) | — | **CS 6601** (strongly rec.) | Algorithms & data structures; strong software dev | Java-equivalent OO | Unity not assumed | Syllabus 2025-spring |
| [CS 7637 — Knowledge-Based AI](cs7637_knowledge-based-ai/readiness-survey.md) | — | Intro AI course | Data structures, OOP, algorithms; Java or Python | — | — | Course page ⏳ |
| [CS 7638 — Robotics: AI Techniques](cs7638_robotics-ai-techniques/readiness-survey.md) | — | ML, CV, or robotics coursework | Python (types, functions, OOP, control flow, exceptions); strong probability & linear algebra; command line | — | — | Course page ⏳ |
| [CS 7639 — Cyber-Physical Design & Analysis](cs7639_cyber-physical-design-and-analysis/readiness-survey.md) | — | — | — | — | CS/Engineering bachelor's or equivalent | Syllabus (current) |
| [CS 7641 — Machine Learning](cs7641_machine-learning/readiness-survey.md) | Intro AI course | — | Statistics, vector calculus, information theory, linear algebra | Prior ML exposure | Contact instructor/TAs if unsure | Syllabus 2025-fall |
| [CS 7642 — Reinforcement Learning](cs7642_reinforcement-learning/readiness-survey.md) | — | **CS 7641** (strongly rec.) | Linear algebra, calculus, statistics; Python, NumPy; PyTorch; Jupyter, Matplotlib | — | — | Course page ⏳ |
| [CS 7643 — Deep Learning](cs7643_deep-learning/readiness-survey.md) | Prior ML course (**CS 7641** equiv) | — | Linear algebra, calculus (partials), probability/statistics; strong Python | CUDA GPU | Not a first ML course | Syllabus 2026-spring |
| [CS 7646 — Machine Learning for Trading](cs7646_machine-learning-for-trading/readiness-survey.md) | — | — | Statistics basics (distributions, central tendency, geo/arithmetic means); strong programming | — | All backgrounds welcome | Course page ⏳ |
| [CS 7650 — Natural Language](cs7650_natural-language/readiness-survey.md) | A data structures course; intro AI or ML course | — | Python | — | Colab Pro recommended | Syllabus 2025-fall |
| [CS 7711 — Health Sensing & Interventions](cs7711_health-sensing-and-interventions/readiness-survey.md) | — | — | Computer w/ Python & Flutter; smartphone | Python | Accommodates limited-programming students | Syllabus 2026-spring |

## CS 8803 Special Topics

| Course | Course Prereq | Rec. Course Prereq | Knowledge (High) | Knowledge (Low) | Exceptions | Source |
|---|---|---|---|---|---|---|
| [CS 8803 O08 — Compilers: Theory & Practice](cs8803-o08_compilers-theory-and-practice/readiness-survey.md) | — | — | Data structures & algorithms; Java or C++; build substantial software; Linux | — | — | Syllabus 2026-spring |
| [CS 8803 O15 — Intro to Computer Law](cs8803-o15_introduction-to-computer-law/readiness-survey.md) | — | — | Java, IDE familiarity | — | GT free Intro to OOP w/ Java offered | Syllabus 2024 ⏳ |
| [CS 8803 O17 — Global Entrepreneurship](cs8803-o17_global-entrepreneurship/readiness-survey.md) | — | — | — | — | — | Course page |
| [CS 8803 O20 — Quantum Hardware](cs8803-o20_quantum-hardware/readiness-survey.md) | — | — | Calculus, complex numbers, linear algebra (vector/inner-product spaces, diagonalization, eigenvalues); computer w/ Python & Qiskit | Prior quantum exposure | No physics needed | Syllabus 2025-summer |
| [CS 8803 O24 — Intro to Research](cs8803-o24_intro-to-research/readiness-survey.md) | — | — | Word processors; learn LaTeX | — | Slack required | Syllabus 2024 ⏳ |
| [CS 8803 O27 — Computer Graphics in the AI Era](cs8803-o27_computer-graphics-in-the-ai-era/readiness-survey.md) | — | **CS 3451** (graphics) | Graphics fundamentals (CS 3451 level); calculus; linear algebra | — | No AI/ML needed; 3 prep lectures | Syllabus 2026-spring |

## CSE / ECE

| Course | Course Prereq | Rec. Course Prereq | Knowledge (High) | Knowledge (Low) | Exceptions | Source |
|---|---|---|---|---|---|---|
| [CSE 6220 — Intro to High-Performance Computing](cse6220_intro-to-high-performance-computing/readiness-survey.md) | — | **CS 6515** (or undergrad algorithms) | Algorithms & data structures w/ big-O (CS 3510 level); C/C++; Unix CLI; calculus, linear algebra, probability | — | — | Syllabus 2025-fall |
| [CSE 6242 — Data and Visual Analytics](cse6242_data-and-visual-analytics/readiness-survey.md) | — | **CSE 6040** (Analytics students) | A high-level lang (Python/C++/Java); debugging; linear algebra, probability, statistics | — | No formal prereqs | Syllabus 2025-fall |
| [CSE 6250 — Big Data for Health Informatics](cse6250_big-data-for-health-informatics/readiness-survey.md) | 🔒 **CS 7641**; grade C in MATH 3215/3225, ECE 3077, or ISYE 2027; two of CX 4240, CS 4400, CX 4242 | — | Scala, Python, Java; ETL (SQL/NoSQL) | — | — | Syllabus 2026-spring |
| [CSE 6742 — Modeling, Simulation, & Military Gaming](cse6742_modeling-simulation-and-military-gaming/readiness-survey.md) | — | — | — | — | — | Course page |
| [ECE 8843 — Side-Channels & Their Role in Cybersecurity](https://omscs.gatech.edu/ece-8843-side-channels-and-their-role-cybersecurity) | — | **ECE 4100/6100** (HPC architecture) | — | C/C++ | Graduate standing; none required | Course page (Jun 2026) |

## ISYE / INTA / MGT / PUBP

| Course | Course Prereq | Rec. Course Prereq | Knowledge (High) | Knowledge (Low) | Exceptions | Source |
|---|---|---|---|---|---|---|
| [INTA 6450 — Data Analytics & Security](inta6450_data-analytics-and-security/readiness-survey.md) | — | — | — | — | No prereqs; approachable w/o programming/statistics | Syllabus 2024 ⏳ |
| [ISYE 6402 — Time Series Analysis](isye6402_time-series-analysis/readiness-survey.md) | — | — | Statistics/probability; programming; linear algebra; calculus; linear regression | — | R used | Syllabus 2026-spring |
| [ISYE 6414 — Regression Analysis](isye6414_regression-analysis/readiness-survey.md) | — | — | Statistics & probability; linear algebra; Python and/or R; Jupyter, Git/GitHub | An IDE | — | Syllabus 2026-summer |
| [ISYE 6420 — Bayesian Statistics](isye6420_bayesian-statistics/readiness-survey.md) | — | — | Intro probability & statistics; programming; calculus | — | — | Syllabus 2026-spring |
| [ISYE 6501 — Intro to Analytics Modeling](isye6501_intro-to-analytics-modeling/readiness-survey.md) | — | — | Probability & statistics; programming; linear algebra; basic calculus | R | — | Syllabus 2023 ⏳ |
| [ISYE 6525 — Topics on High-Dimensional Data Analytics](isye6525_topics-on-high-dimensional-data-analytics/readiness-survey.md) | — | — | Regression & linear algebra; programming (Python/R/Matlab) | — | — | Syllabus 2026-spring |
| [ISYE 6644 — Simulation & Modeling for Engineering & Science](isye6644_simulation-and-modeling-for-engineering-and-science/readiness-survey.md) | — | — | Basic calculus, probability, statistics | Programming (e.g., Excel) | Bootcamps provided | Syllabus 2026-spring |
| [ISYE 6669 — Deterministic Optimization](isye6669_deterministic-optimization/readiness-survey.md) | — | — | Linear algebra; multivariate calculus; basic probability; programming (Python) | — | — | Syllabus 2025-spring |
| [MGT 6311 — Digital Marketing](mgt6311_digital-marketing/readiness-survey.md) | — | — | — | — | — | Course page |
| [MGT 8813 — Financial Modeling](mgt8813_financial-modeling/readiness-survey.md) | — | **MGT 8803/6754** | Excel w/ Analysis ToolPak & Solver | — | — | Syllabus 2026-summer |
| [PUBP 6725 — Information Security Policies](pubp6725_information-security-policies/readiness-survey.md) | — | — | Computers & data networking basics; protocols & vulnerabilities exposure | Economics; public policy | — | Syllabus 2026-spring |
| [PUBP 8823 — Geopolitics of Cybersecurity](pubp8823_geopolitics-of-cybersecurity/readiness-survey.md) | — | — | — | Engineering or strategic cybersecurity foundations (cryptography, security engineering, network security, public policy, international security) | No formal prereqs | Syllabus 2026-spring |
