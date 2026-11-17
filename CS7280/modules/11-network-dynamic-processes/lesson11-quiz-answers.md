# Lesson 11 — Quiz Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results (7/7, 100%)

Questions: [[lesson11-quiz]].

---

**Q1** (robustness statements):
1. True — For a power-law network under random failures, $f_c$ decreases as $\gamma$ increases
2. False — The Molloy-Reed criterion is applicable to any network
3. False — Power-law networks disintegrate into multiple components after removing only a few random nodes
4. True — Random node removal causes a larger decrease in the giant component than random removal of the same fraction of edges

**Q2** (power-law network with exponent $\gamma$, minimum degree $k_{min}$, threshold $f_c$):
1. False — In the case of attacks, $f_c$ for $k_{min}=3$ is less than $f_c$ for $k_{min}=2$
2. False — In the case of random failures, $f_c$ increases as $\gamma$ increases
3. True — In the case of attacks, for $k_{min}=3$, $f_c$ increases as $\gamma$ increases
4. True — For the same $k_{min}$, the thresholds for random failures and attacks become asymptotically equal as $\gamma$ increases

**Q3** (Kleinberg's model, 3-dimensional grid with $q = 2$): There will be a large fraction of links covering long distances

**Q4** (Kuramoto critical coupling strength $K_c$): $\frac{2}{\pi\Omega}$

**Q5** (consensus formation in adaptive networks):
1. True — In an adaptive network, global consensus is harder to reach for high tolerance values
2. False — When tolerance is low, smaller consensus clusters form in the adaptive network than in the static network
3. False — Global consensus is easier to achieve in the adaptive network
4. True — Large consensus clusters are obtained even at low tolerance in adaptive networks

**Q6** (adaptive topological change): Joe following Leila

**Q7** (decentralized search in the two regular networks):
1. False — For network (a), the probability of random "shortcut links" should decay with $d(v, w)^{-2}$
2. True — For network (a), the probability of random "shortcut links" should decay with $rank_v(w)^{-1}$
3. True — For network (b), the probability of random "shortcut links" should decay with $d(v, w)^{-2}$
4. False — For network (b), the probability of random "shortcut links" should decay with $rank_v(w)^{-2}$
