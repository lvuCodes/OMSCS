# Lesson 13 — Knowledge Check Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results

Questions: [[lesson13-knowledge-check]].

---

**Q1** (capture-recapture size estimate): $150 \pm 0$

**Q2** (inclusion probability under link-tracing sampling): [^l13-2]
1. False — Nodes with high degree are more likely to be included in the sample than nodes with low degree but high betweenness centrality.
2. True — The probability that a node is NOT included in the sample drops exponentially with its betweenness centrality.
3. True — Swapping the set of sources with the set of targets, while maintaining their number, gives the same node and edge inclusion probabilities.
4. False — Doubling the number of target nodes will, approximately, double the probability that an edge is sampled.

**Q3** (Horvitz-Thompson estimator):
1. False — For degree-2 node counts under incident subgraph sampling, count the degree-2 nodes in the sample and multiply by $N/n$.
2. True — For degree-2 node counts under induced subgraph sampling, count the degree-2 nodes in the sample and multiply by $N/n$.
3. True — For average degree with traceroute sampling, the estimator gives lower weight to nodes with higher betweenness centrality.
4. False — The Horvitz-Thompson estimator can be applied for any given sample of nodes.

**Q4** (link prediction with logistic regression):
1. True — We need to know certain node pairs that are connected and certain other node pairs that are not connected.
2. False — We need at least one metric defined on node attributes and at least one topological similarity metric for node pairs.
3. False — The logistic regression coefficients are different for each node pair.
4. True — This framework can also be applied when we have no information about node attributes.

**Q5** (inference of association networks):
1. False — When two genes X and Y are highly correlated, we can infer that X regulates Y.
2. True — Pearson's correlation coefficient mostly captures linear dependencies.
3. False — A very high correlation coefficient (say 99%) guarantees statistical significance and a very low p-value.
4. True — With $m=10000$ node pairs, a False Discovery Rate $\alpha = 10^{-6}$, and a lowest correlation p-value of 0.05, the resulting association network will not have any edges.

**Q6** (examples of association network inference):
1. True — Estimating connectivity between brain regions of interest from functional activity measurements.
2. False — Inferring a package delivery network from edge-node order and receipt dates.
3. False — Completing the missing connections of a customer-product bipartite network for recommendation.
4. True — Building a citation network from a set of scientific papers.

[^l13-2]: Possible source issue, see [[lesson-errata#L13-2|errata L13-2]].
