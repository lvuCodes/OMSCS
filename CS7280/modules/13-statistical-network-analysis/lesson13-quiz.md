# Lesson 13 — Quiz (graded)

> Source: Canvas — CS-7280-O01, OAN (Summer 2026)

Combined view of the seven graded quiz questions. For multiple true/false questions, consider each item as its own separate, independent statement. See also [[lesson13-quiz-all.pdf]].

---

### Q1 — Multiple choice (1 point)

Suppose that you decide to use the capture-recapture method to estimate the size of a network. The size of the first sample (the "marked sample") is 100 nodes, the size of the second sample is 150 nodes, the intersection of the two samples is 100 nodes. Which of the following is a valid reason to be skeptical of this estimate? You can assume that the size of the network is much larger than 150 nodes.

- [ ] The capture-recapture estimator is only applicable when the intersection of the two samples is much lower than the size of each sample.
- [ ] The two samples are too small.
- [ ] The variance of an estimate can never be zero.
- [ ] The two samples are probably not independent.

---

### Q2 — Multiple choice (1 point)

This question refers to network sampling strategies. Which of the following statements is TRUE?

- [ ] With snowball sampling, the sampled nodes will be in the same connected component.
- [ ] With induced subgraph sampling it is possible to sample the same edge more than once.
- [ ] With traceroute sampling, all nodes in the sample will have degree larger than one.
- [ ] With incident subgraph sampling some nodes may have zero inclusion probability.

---

### Q3 — Fill in the Blank (1 point)

The following question refers to the Horvitz-Thompson estimator. Which of the following statements is/are TRUE?

1. Suppose that we are not aware of the Horvitz-Thompson estimator. So we estimate the mean degree of the network by taking the average of all node degrees collected with star sampling (i.e., the degrees of the seed nodes). We would still end up with the correct formula. — `True` / `False`
2. Suppose that we are not aware of the Horvitz-Thompson estimator. So we estimate the mean degree of the network by taking the average of all node degrees collected with traceroute sampling. We would still end up with the correct formula. — `True` / `False`
3. Suppose that we are not aware of the Horvitz-Thompson estimator. So we estimate the mean degree of the network by taking the average of all node degrees collected with induced subgraph sampling. We would still end up with the correct formula. — `True` / `False`
4. Suppose that we are not aware of the Horvitz-Thompson estimator. So we estimate the mean degree of the network by taking a random sample of nodes WITH replacement and then averaging their degrees. We would still end up with the correct formula. — `True` / `False`

---

### Q4 — Multiple choice (1 point)

This question refers to the method we presented for the estimation of the size of a network using traceroute-like sampling. Suppose that whenever we ignore a target, we can always observe that target in traceroutes to other targets. Which of the following statements is TRUE?

- [ ] In expectation, the estimated network size is equal to the number of observed nodes.
- [ ] The estimated network size depends on the number of targets but not on the number of sources.
- [ ] The estimated network size is larger than the number of observed nodes.
- [ ] Since we can observe each target in our sample even if it is not included as a target, we can conclude that all non-source nodes are targets.

---

### Q5 — Fill in the Blank (1 point)

This question refers to the inference of association networks, as presented in this Lesson. Note: Let $n$ be the number of nodes. Which of the following statements is/are TRUE?

1. Negative correlations imply that the nodes should not be connected. — `TRUE` / `FALSE`
2. The Fisher-transformed correlation value of two random vectors follows a Gaussian distribution with zero mean and variance $1/(n-3)$. — `TRUE` / `FALSE`
3. The Multiple Testing problem is harder in network inference than in other contexts because the involved statistical tests are typically not independent. — `TRUE` / `FALSE`
4. The association network inference framework, as presented in this Lesson, can also be applied in directed networks. — `TRUE` / `FALSE`

---

### Q6 — Fill in the Blank (1 point)

This question relates to the network tomography. Which of the following statements is/are TRUE?

1. Topology inference using network tomography (with multiple nodes acting as sources) is only applicable on tree networks. — `True` / `False`
2. Often, network tomography results in under-constrained systems of equations that have multiple possible solutions. — `True` / `False`
3. One specific network tomography problem is to use per-link flow measurements to calculate end-to-end flows. — `True` / `False`
4. It is always possible to accurately infer the topology of a tree network using the hierarchical clustering tomography method presented in this lesson, as long as the tree is binary and we have enough measurements to the given (i.e., fixed) set of destinations. — `True` / `False`

---

### Q7 — Fill in the Blank (1 point)

This question refers to the localization of congested links used end-to-end path measurements. The following figure shows a network topology in which squares 1, 2, 3, 4 are four users, circles A-F are 6 network nodes, green edges are connections between network nodes, and red paths indicate the route for each pair of users. Based on the figure which of the following statements is/are True?

![[img/quiz-q07-topology.png|500]]

1. If we detect performance problems between (2, 3), while all other routes are normal, link (C, D) is most likely congested. — `True` / `False`
2. If we detect performance problems between (1, 2), while all other routes are normal, link (B, D) is most likely congested. — `True` / `False`
3. If we detect performance problems between (1, 3), we should also be able to detect performance problems between (3, 4). — `True` / `False`
4. If we detect performance problems between (1, 4), we should also be able to detect performance problems between (1, 2). — `True` / `False`
