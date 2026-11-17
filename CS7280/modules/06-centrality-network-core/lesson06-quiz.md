# Lesson 6 — Quiz (graded)

> Source: Canvas — CS-7280-O01, OAN (Summer 2026)

Combined view of the six graded quiz questions. See also [[lesson06-quiz-all.pdf]]. The answer key is in [[lesson06-quiz-answers]].

---

### Q1 — Fill in the Blank (1 point)

Which of the following statement(s) about Eigenvector centrality and Katz centrality is/are True:

1. The Eigenvector centrality accounts for not only the centrality of the node but also the centrality of all the neighbors of the node. — `True` / `False`
2. The Eigenvector centrality is typically used for directed graphs. — `True` / `False`
3. It is possible to have the Eigenvector centrality value of a node to be zero. — `True` / `False`
4. The Katz centrality metric is typically used for undirected graphs. — `True` / `False`

---

### Q2 — Multiple choice (1 point)

The organization of a large company can be represented as a network based on the relationship of employees. Which centrality metric would be the most suitable to find the members who are central to the functioning of this company? The centrality metric should be appropriate for undirected networks and should not require any extraneous parameters. (Hint: Consider the employees in the company as nodes and undirected edges represent collaborations between employees)

- [ ] Degree Centrality
- [ ] Eigenvector Centrality
- [ ] Katz Centrality
- [ ] Pagerank Centrality

---

### Q3 — Multiple choice (1 point)

In many problems, we are interested in the distance between two nodes. Which of the following path-based centrality metrics is the best in the case of highly sparse networks?

- [ ] Closeness Centrality
- [ ] Harmonic Centrality
- [ ] Betweenness Centrality
- [ ] Path Centrality

---

### Q4 — Multiple choice (1 point)

Which of the following nodes in the figure has the largest "Shortest path betweenness centrality"?

![[img/q04-betweenness-network.png|300]]

- [ ] A
- [ ] B
- [ ] C
- [ ] D

---

### Q5 — Multiple choice (1 point)

Identify the $k$-core decomposition of the following graph:

![[img/q05-kcore-graph.png|400]]

- [ ] Option A
![[img/q05-option-a.png|400]]
- [ ] Option B
![[img/q05-option-b.png|400]]
- [ ] Option C
![[img/q05-option-c.png|400]]
- [ ] Option D
![[img/q05-option-d.png|400]]

---

### Q6 — Fill in the Blank (1 point)

Which of the following statements are TRUE about the rich club of a network:

1. The rich club of a network always exists. — `True` / `False`
2. The rich club coefficient is a function of the degree of the set of nodes in the rich club. — `True` / `False`
3. The rich club coefficient may be statistically significant for more than one value of $k$. — `True` / `False`
4. The rich club coefficient is determined by comparison with networks of the same number of nodes and edges. — `True` / `False`
