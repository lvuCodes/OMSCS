# Lesson 8 — Quiz Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results (5.75/7, 82.14%)

Questions: [[lesson08-quiz]].

---

**Q1** (participation coefficient statements, TRUE/FALSE) — 0.75/1:
1. False — a participation coefficient of 1 represents the highest connectivity of a node to other nodes in its own community
2. True — a participation coefficient of almost 1 can be seen for a node with very large degree when its connections are uniformly distributed among all communities
3. True — a participation coefficient of 0 means that the node is not a member of any community ❌ *(correct: False — a coefficient of 0 means all of the node's links are within its own community)*
4. True — a high participation coefficient indicates that the node acts as a bridge between its own community and other communities

**Q2** (within-module-degree — identify the hubs of the Green and Blue communities, select two): **1 and 4** *(answered 1 & 3 — incorrect)*

**Q3** (runtime-complexity statements, TRUE/FALSE) — 1/1:
1. True — Cfinder has the highest worst-case runtime complexity
2. False — Louvain runtime complexity is higher in sparse networks
3. True — actual runtime complexity rankings of various algorithms can change depending on the size (number of nodes) of the network
4. False — runtime complexity is a useful metric for computation timings when running these algorithms on very small networks

**Q4** (Cfinder algorithm statements, TRUE/FALSE) — 1/1:
1. False — the Cfinder algorithm is based on modularity maximization
2. False — a node that belongs to $m$ communities participates in at most $m$ $k$-cliques
3. True — a node that belongs to $m$ communities participates in at least $m$ $k$-cliques
4. False — if two $k$-cliques belong in the same community, they must share $k-1$ links

**Q5** (CFinder critical density threshold — max edges for $n=200$, $k=3$): **995**

**Q6** (node-type labeling from participation coefficient × within-module degree): **Connector Hub = 4, Provincial Hub = 1, Connector node = 3, Peripheral node = 2**

**Q7** (which node has the highest participation coefficient): **E**
