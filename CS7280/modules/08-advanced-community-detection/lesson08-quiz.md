# Lesson 8 — Quiz (graded)

> Source: Canvas — CS-7280-O01, OAN (Summer 2026)

Combined view of the seven graded quiz questions. See also [[lesson08-quiz-all.pdf]].

---

### Q1 — Fill in the Blank (1 point)

Which of the following statements about the participation coefficient is/are TRUE:

1. A participation coefficient of 1 represents the highest connectivity of a node to other nodes in its own community. — `True` / `False`
2. A participation coefficient of almost 1 can be seen for a node with very large degree when its connections are uniformly distributed among all communities. — `True` / `False`
3. A participation coefficient of 0 means that the node is not a member of any community. — `True` / `False`
4. A high participation coefficient indicates that the node acts as a bridge between its own community and other communities. — `True` / `False`

---

### Q2 — Multiple answer (1 point)

Based upon your understanding of the within-module degree, identify the hubs for the two Green and Blue communities, without calculating the actual value (i.e., select two of the following four answers).

![[img/q02-within-module-degree-network.png|450]]

- [ ] 1
- [ ] 2
- [ ] 3
- [ ] 4

---

### Q3 — Fill in the Blank (1 point)

Mark each of the following statements about runtime complexity as True or False:

1. CFinder has the highest worst-case runtime complexity. — `True` / `False`
2. Louvain runtime complexity is higher in sparse networks. — `True` / `False`
3. Actual runtime complexity rankings of various algorithms can change depending on the size (number of nodes) of the network. — `True` / `False`
4. Runtime complexity is a useful metric for computation timings when running these algorithms on very small networks. — `True` / `False`

---

### Q4 — Fill in the Blank (1 point)

Mark each of the following statements about the CFinder algorithm as True or False:

1. The CFinder algorithm is based on modularity maximization. — `True` / `False`
2. A node that is found to belong to $m$ communities participates in at most $m$ $k$-cliques. — `True` / `False`
3. A node that is found to belong to $m$ communities participates in at least $m$ $k$-cliques. — `True` / `False`
4. If two $k$-cliques belong in the same community, they must share $k-1$ links. — `True` / `False`

---

### Q5 — Multiple choice (1 point)

In the lesson, we learned about the critical density threshold for the CFinder algorithm. Suppose you are given a graph with $n=200$ nodes. You plan to identify its communities using the CFinder algorithm with $k=3$. What is the maximum number of edges in the graph so that you can reliably apply this community detection method? (Hint: please select the closer integer below.)

- [ ] 340
- [ ] 350
- [ ] 1000
- [ ] 995

---

### Q6 — Multiple choice (1 point)

In the lesson, we learned that the interplay of participation coefficient and within-module degree help us identify four types of nodes. For the given network, which of the following statement labels nodes 1 to 4 correctly? (Hint: you do not need to compute actual values.)

![[img/q06-node-types-network.png|450]]

- [ ] Connector Hub = 3, Provincial Hub = 1, Connector node = 4, Peripheral node = 2
- [ ] Connector Hub = 4, Provincial Hub = 1, Connector node = 2, Peripheral node = 3
- [ ] Connector Hub = 4, Provincial Hub = 1, Connector node = 3, Peripheral node = 2
- [ ] Connector Hub = 1, Provincial Hub = 4, Connector node = 3, Peripheral node = 2

---

### Q7 — Multiple choice (1 point)

Which node has the highest participation coefficient?

![[img/q07-participation-coefficient-network.png|450]]

- [ ] C
- [ ] E
- [ ] G
- [ ] I
