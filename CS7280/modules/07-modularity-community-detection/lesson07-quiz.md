# Lesson 7 — Quiz (graded)

> Source: Canvas — CS-7280-O01, OAN (Summer 2026)

Combined view of the six graded quiz questions. See also [[lesson07-quiz-all.pdf]].

---

### Q1 — Multiple choice (1 point)

Given the following dendrogram, identify the communities at the given "horizontal cut" (dashed line).

![[img/q01-dendrogram-cut.png|450]]

- [ ] (A, B, C, D, E), (F, G), (H, I)
- [ ] (A, B, C), (D, E), (F, G), (H, I)
- [ ] (A, B, C, D), (E), (F, G), (H, I)
- [ ] (A, B, C, D), (E), (F, G, H, I)

---

### Q2 — Multiple choice (1 point)

Which of the statements regarding the modularity metric is FALSE:

- [ ] The modularity metric quantifies the density of internal edges in a given set of communities, relative to the corresponding density in degree-preserving randomized networks.
- [ ] The modularity metric cannot be applied in overlapping communities.
- [ ] The modularity metric directly penalizes any edges between different communities.
- [ ] The modularity metric may also be negative.

---

### Q3 — Multiple choice (1 point)

Compute the modularity metric for the given network and community partition.

![[img/q03-modularity-network.png|400]]

- [ ] 0.251
- [ ] 0.758
- [ ] 0.367
- [ ] 0.718

---

### Q4 — Multiple choice (1 point)

Which of the following statements about the complexity of the greedy modularity maximization algorithm is TRUE:

- [ ] Inspecting each link and then computing the modularity difference requires $O(L \cdot K)$ computations, where $L$ is the number of links and $K$ is the number of operations to calculate the modularity difference.
- [ ] The algorithm always performs $N$ community mergings.
- [ ] For a dense graph the run time complexity is $O(N^2)$.
- [ ] With appropriate data-structures the run time complexity can be reduced to $O(N \log N)$.

---

### Q5 — Multiple choice (1 point)

Which of the following statements about modularity maximization and modularity resolution is FALSE:

- [ ] It is possible that the modularity increases when merging two communities into a single community, even if they are distinct communities.
- [ ] During the process of maximizing the modularity $M$, a single link between two communities is not sufficient to merge them.
- [ ] Modularity maximization cannot detect communities that are smaller than the resolution limit.
- [ ] Modularity maximization forces some small communities into larger ones.

---

### Q6 — Multiple choice (1 point)

Which statement(s) regarding modularity is true for the following network?

![[img/q06-community-network.png|450]]

- [ ] Merging communities B and D will increase modularity.
- [ ] Merging communities B and C will increase modularity.
- [ ] Merging communities C and D will increase modularity.
- [ ] Merging communities A and B will increase modularity.
