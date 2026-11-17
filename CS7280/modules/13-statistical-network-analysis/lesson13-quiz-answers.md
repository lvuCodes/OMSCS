# Lesson 13 — Quiz Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results (6.5/7, 92.86%)

Questions: [[lesson13-quiz]].

---

**Q1** (skepticism about a capture-recapture size estimate): The two samples are probably not independent.

**Q2** (which statement about network sampling strategies is TRUE): With incident subgraph sampling some nodes may have zero inclusion probability.

**Q3** (Horvitz-Thompson estimator):
1. True — star sampling (averaging the degrees of the seed nodes) still yields the correct formula
2. False — traceroute sampling does not yield the correct formula
3. False — induced subgraph sampling does not yield the correct formula
4. False — a random sample of nodes WITH replacement, averaged, does not yield the correct formula ❌ *(answered "True" — incorrect)*

**Q4** (network size estimation with traceroute-like sampling, when an ignored target is still observed via other traceroutes): In expectation, the estimated network size is equal to the number of observed nodes.

**Q5** (inference of association networks): [^l13-4]
1. FALSE — negative correlations do not imply the nodes should not be connected
2. FALSE — the Fisher-transformed correlation of two random vectors is not Gaussian with zero mean and variance $1/(n-3)$
3. TRUE — the Multiple Testing problem is harder in network inference because the involved tests are typically not independent
4. FALSE — the framework as presented does not apply to directed networks

**Q6** (network tomography): [^l13-1]
1. False — topology inference with multiple sources is not restricted to tree networks
2. True — tomography often yields under-constrained systems with multiple solutions
3. False — using per-link flow measurements to calculate end-to-end flows is not a network tomography problem ❌ *(answered "True" — incorrect)*
4. False — accurate topology inference of a binary tree is not always possible with the hierarchical clustering tomography method, even with enough measurements to a fixed destination set

**Q7** (localizing congested links from end-to-end path measurements):
1. True — problems only between (2, 3) implicate link (C, D)
2. False — problems only between (1, 2) do not implicate link (B, D)
3. False — problems between (1, 3) do not imply problems between (3, 4)
4. False — problems between (1, 4) do not imply problems between (1, 2)

[^l13-1]: Possible source issue, see [[lesson-errata#L13-1|errata L13-1]].
[^l13-4]: Possible source issue, see [[lesson-errata#L13-4|errata L13-4]].
