# CS 6340 — Spring 2025 Syllabus

Source: `downloads/CS 6340 2025-1.pdf` (OMSCS sample syllabus for the Spring 2025 offering; the document body header reads "Fall 2024," a carried-over template label).

## Instructional Staff

- Instructors: Mayur Naik, Chris Poch
- Head TAs: Kelly Parks, Joel Cooper
- Teaching Assistants: John Daniel, Joseph Dougherty, Joseph Knaack, Susie Lin, Samantha Llewellyn, Justin McLellan, Kevin Windbigler

## Course Overview

The course explores software analysis — determining whether software is correct and finding bugs ahead of users. It covers how development environments detect issues (e.g., unused variables) before compilation and how strongly typed languages prevent bugs. With testing, debugging, and security assessment now taking more resources than development itself, the industry increasingly relies on tools to write better software. The course investigates multiple analysis techniques and their limits, with most lectures accompanied by hands-on labs. Techniques include dataflow analysis, constraint-based analysis, type systems, automated test-case generation, and symbolic execution.

## Prerequisites

Fluency in a C-family language (C, C++, Java, or C#) is expected; most classwork is in C++, and the effort required is greatly increased without C-family fluency. A C++ Primer highlights the language features used in the labs. Familiarity with basic computer science and mathematics concepts and with UNIX-like environment tooling is assumed. A Readiness Assessment (see [readiness-survey.md](readiness-survey.md)) is available to identify prerequisite tasks to learn or re-familiarize with before enrolling.

## Required Text

No required text. Several recommended books covering various sections are listed at [rightingcode.github.io/books.html](https://rightingcode.github.io/books.html). Students who struggle with discrete-math notation often find Chapter 0 of Michael Sipser's *Introduction to the Theory of Computation* helpful.

## Grading

| Weight | Component |
|---|---|
| 60% | Labs — Lab 0 (4%) and seven other labs (8% each) |
| 20% | Course Exam — Introduction to Software Analysis, Introduction to Software Testing, Automated Test Generation, Pointer Analysis |
| 20% | Quizzes, Surveys, and Participation — beginning/mid/end surveys (0.5% each), syllabus quiz (2%), per-lesson quizzes (1.5% each), Ed participation (0.05 pts per meaningful post, capped at 5%) |

Scores are not curved individually; letter grades are at the instructors' discretion, with total-score ranges released after the exam to scale for difficulty. Georgia Tech does not assign plus/minus grades (only A, B, C, D, F, W, I). No make-up assignments, extra credit, or "pity points."

## Technical Requirements

Meet or exceed OMSCS program requirements: at least 8 GB RAM and an x64 processor for a decent VM experience. Apple M-series processors are permitted, but some labs may require additional setup and peer support (no TAs currently use M-series). Labs are only supported via a Docker image or the course VM — not directly on host hardware (LLVM is difficult to run correctly). Exams via Honorlock require a relatively current Chrome browser.

## Additional Sections

The full syllabus also covers: course objectives, course schedule, lessons and lesson quizzes, course forum, office hours, lab assignments / development environment / Gradescope, quizzes and exams, Ed Discussions participation, regrade requests, deadlines and extensions, academic integrity (collaboration, plagiarism, penalties, source control), and disability services. Consult the source PDF for these details.
