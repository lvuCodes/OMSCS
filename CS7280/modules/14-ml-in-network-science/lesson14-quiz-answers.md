# Lesson 14 — Quiz Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results (5.75/6, 95.83%)

Questions: [[lesson14-quiz]].

---

**Q1** (fixed-length random-walk node embeddings — node2vec, DeepWalk):
1. False — the conditional probability of visiting $v$ on a length-$T$ walk from $u$ is not calculated analytically
2. True — those conditional probabilities are computed numerically, by simulating random walks of length $T$ from each node $u$
3. False — softmax is not the only formula that can express those conditional probabilities
4. True — at $T = 1$ hop the random-walk method is asymptotically equivalent to adjacency-based node embeddings

**Q2** (classifying majors from one labeled node per class, with homophily): Compute random-walk node embeddings (with a length that is more than 1 but much less than the network diameter), and classify each node based on the shortest distance between its embedding vector and the embedding vectors of the three labeled nodes.

**Q3** (GNN in the polypharmacy application):
1. False — a separate parameter matrix per neighbor of $v$ is not needed
2. True — a separate parameter matrix is needed for each type of edge that $v$ connects to
3. False — the layer-$k$ embedding of $v$ can be computed without knowing the target proteins of $v$
4. True — the embedding of $v$ can still be computed from its target proteins alone, with no known drug-interaction side-effects

**Q4** (inductive ability of GNNs): [^l14-2]
1. True — it is feasible because the same trainable parameters are used for all nodes
2. True — it assumes the training nodes share the statistical properties of the rest of the nodes
3. True — it increases with the number of nodes used in training ❌ *(answered "False" — incorrect)*
4. True — it also applies to future nodes added to the network after training

**Q5** (GNN node classification on a social network with partial labels and full node attributes):
1. True — the layer-0 embeddings are equal to the node features
2. True — a layer-3 embedding depends on the layer-2 embeddings of that node's neighbors
3. False — the training data should not consist of all nodes with a known political affiliation
4. True — more layers (greater depth) makes the network more susceptible to overfitting

**Q6** (minimum temporal spanning tree originating at node-A): the third option — ![[img/quiz-q06-option-3.png|300]]

[^l14-2]: Possible source issue, see [[lesson-errata#L14-2|errata L14-2]].
