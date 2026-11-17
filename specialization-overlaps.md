# OMSCS Course Overlaps

Courses that count toward more than one specialization, with the role each course plays per specialization. Derived from the six specialization requirement pages and scoped to courses **offered online through OMSCS**, per the [current-courses listing](available-courses/current-courses.md).

## Legend

**Specializations:**

- **CPR** — Computational Perception and Robotics
- **Graphics** — Computer Graphics
- **Systems** — Computing Systems
- **HCI** — Human-Computer Interaction
- **AI** — Artificial Intelligence (formerly Interactive Intelligence)
- **ML** — Machine Learning

**Role values:**

- **Core** — counts toward the specialization's core requirement
- **Elec** — counts as a specialization elective
- **Core+Elec** — listed as both a core option and an elective within the same specialization
- **—** — not part of that specialization

## Courses Shared Across Specializations

| Course                                                    | CPR  | Graphics  | Systems | HCI  | AI   | ML   | Core Count |
| --------------------------------------------------------- | ---- | --------- | ------- | ---- | ---- | ---- | ---------- |
| CS 6515 Introduction to Graduate Algorithms               | Core | Core      | Core    | —    | Core | Core | 5          |
| CS 7641 Machine Learning                                  | Core | —         | —       | —    | Core | Core | 3          |
| CS 6300 Software Development Process                      | —    | —         | Core    | —    | Core | —    | 2          |
| CS 6601 Artificial Intelligence                           | Core | —         | —       | —    | Core | —    | 2          |
| CS 6457 Video Game Design                                 | —    | Core+Elec | —       | Elec | —    | —    | 1          |
| CS 6750 Human-Computer Interaction                        | —    | —         | —       | Core | Elec | —    | 1          |
| CS 6440 Introduction to Health Informatics                | —    | —         | —       | Elec | Elec | —    | 0          |
| CS 6460 Educational Technology: Conceptual Foundations    | —    | —         | —       | Elec | Elec | —    | 0          |
| CS 6475 Computational Photography                         | Elec | Elec      | —       | —    | —    | —    | 0          |
| CS 6476 Computer Vision                                   | Elec | Elec      | —       | —    | Elec | Elec | 0          |
| CS 6603 AI, Ethics, and Society                           | —    | —         | —       | —    | Elec | Elec | 0          |
| CS 6795 Introduction to Cognitive Science                 | —    | —         | —       | Elec | Elec | —    | 0          |
| CS 7280 Network Science                                   | —    | —         | Elec    | —    | —    | Elec | 0          |
| CS 7632 Game AI                                           | —    | —         | —       | Elec | Elec | —    | 0          |
| CS 7643 Deep Learning                                     | —    | —         | —       | —    | Elec | Elec | 0          |
| CS 7650 Natural Language                                  | Elec | —         | —       | —    | Elec | Elec | 0          |

## Overlap Notes

**Core in every specialization that uses it:** CS 6515 is the only algorithms-core option offered online, and counts as core across all five specializations that require an algorithms course (CPR, Graphics, Systems, AI, ML). CS 7641 is core across three specializations (CPR, AI, ML).

**Elective in one specialization, core in another:**

- **CS 6750** — core for HCI, but an elective for AI

**Both core and elective within the same specialization** (single-specialization, not shown above): CS 6491 Foundations of Computer Graphics (Graphics), CS 7496 Computer Animation (Graphics), and CS 7470 Mobile and Ubiquitous Computing (HCI) are each listed as both a core option and an elective in that one specialization. CS 6457 Video Game Design is core-and-elective in Graphics and additionally an elective in HCI.

## Recommended Sequencing: Statistics to AI/ML Track

A prerequisite-aware order for the statistics-to-machine-learning path, building foundations before the two heaviest CS courses. CS 7641 and CS 6601 are AI/ML core-overlap courses from the table above; the three ISYE courses are statistics foundations that supply the probability, statistics, and regression background those courses assume.

| Order | Course | Rationale |
| ----- | -------------------------------------- | ------------------------------------------------------------------------------- |
| 1     | ISYE 6501 Intro to Analytics Modeling  | Lowest-barrier on-ramp; broad modeling survey that builds probability/statistics intuition. |
| 2     | ISYE 6414 Regression Analysis          | Statistical-modeling backbone for ML; reinforces linear algebra and statistics. |
| 3     | ISYE 6420 Bayesian Statistics          | Adds probabilistic depth and calculus maturity used by ML's probabilistic methods. |
| 4     | CS 6601 Artificial Intelligence        | Recommended prerequisite for CS 7641; applies the accumulated math and adds search/representation. |
| 5     | CS 7641 Machine Learning               | Capstone of the set; leverages regression (6414), Bayesian/probability (6420), and introductory AI (6601). |

**Sequencing logic.** The statistics track (6501 → 6414 → 6420) ascends in rigor; the CS track (6601 → 7641) follows the published prerequisite chain. The ordering also keeps the two highest-workload courses (CS 6601, CS 7641) last and separated rather than stacked in one term.

**Adjustment by bottleneck.** Steps 1–3 are the clearest fixed sequence, with ISYE 6501 first. For a strong programmer who is light on mathematics, CS 6601 may move earlier (its real barrier is Python/algorithms, not statistics) — but CS 7641 remains last. CS 6601 and CS 7641 should not share a term.

Last Updated: Jun 22, 2026
