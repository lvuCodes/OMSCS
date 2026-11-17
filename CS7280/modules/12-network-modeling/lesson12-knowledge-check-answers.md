# Lesson 12 — Knowledge Check Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results

Questions: [[lesson12-knowledge-check]].

---

**Q1** (link-copy model differential equation for $m=2$): $\frac{dx_j}{dt} = \frac{2p}{t} + \frac{qx_j}{t}$

**Q2** (generating the given network with different models):
1. False — It is possible to generate this network with the optimization-based model with cost function $C_j = d_{i,j} + h_j$.
2. False — It is possible to generate this network with the optimization-based model with cost function $C_j = 0.1 d_{i,j} + h_j$.
3. True — When adding node 4, the link-copy model with $p=1/2$ assigns higher probability to edge (4, 0) than linear preferential attachment.
4. False — When adding node 5, the link-copy model with $p=1/2$ assigns higher probability to edge (5, 0) than linear preferential attachment.

**Q3** (rewiring algorithm for degree correlations, multi-edges prohibited):
1. True — We can apply that algorithm to make the network more assortative.
2. False — We can apply that algorithm to make the network more disassortative.
3. True — In the original network, the higher-degree nodes have lower average neighbor degree.
4. False — If the network is rewired to become maximally assortative, the higher-degree nodes will have higher average neighbor degree.

**Q4** (Hierarchical Random Graph model with the given dendrogram):
1. True — The maximum-likelihood estimate of $x$ is $\frac{2}{3}$.
2. True — With $x=\frac{2}{3}$, the likelihood of the model is $\frac{1}{27}$.
3. False — The given dendrogram is optimal; we cannot increase the likelihood of the model with another dendrogram.
4. True — Swapping the position of nodes C and D in the dendrogram will not change the model's likelihood.

**Q5** (MCMC and the optimal HRG dendrogram):
1. True — Comparing $L(D)$ with $L(D')$ is equivalent to comparing $L(D_r)$ with $L(D_r')$, where $D_r$ is the sub-tree of $D$ rooted at the parent of $r$.
2. True — If $L(D') \leq L(D)$, we may accept $D'$ with probability $\frac{L(D')}{L(D)}$.
3. False — The main reason we use MCMC is that it gives us a way to examine all possible dendrograms.
4. True — If $D'$ is sampled by MCMC $N$ times, then $D$ is expected to be sampled about $N \frac{L(D)}{L(D')}$ times.

**Q6** (statements about the lesson's network models):
1. False — In the linear PA model a late node can never become the largest-degree hub, but this is not true for the non-linear PA model with large $\alpha$.
2. False — The Link-Copy model offers a less flexible mechanism to generate power-law networks compared to the PA model.
3. False — After rewiring to create an assortative network, the average neighbor node degree as a function of node degree will be a monotonically increasing function.
4. True — The Hierarchical Graph Model captures various properties of real-world networks, but requires the estimation of a large number of parameters as well as a dendrogram.
