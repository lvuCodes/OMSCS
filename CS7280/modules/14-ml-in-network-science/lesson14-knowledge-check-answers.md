# Lesson 14 — Knowledge Check Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results

Questions: [[lesson14-knowledge-check]].

---

**Q1** (magnitude of the embedding dimension $d$ — select all):
- The higher $d$ is, the closer the similarity of two node embeddings to the network similarity of the corresponding nodes.
- If $d$ is not high enough, it may be that two pairs of nodes have almost the same dot product even though they are not equally similar.

**Q2** (GNN architecture — select all): The dimensionality of the matrices $W_k$ and $B_k$ is $d_k \times d_{k-1}$, where $d_k$ is the embedding dimensionality at layer $k$.

**Q3** (cross-entropy loss for binary node classification — select all):
- The loss function is close to 0 whenever the model predicts correctly the label of a node.
- The loss function assumes that the activation function $\sigma$ varies between 0 and 1.

**Q4** (decoder in the polypharmacy GNN — select all): It predicts whether an edge of a given type exists between two given drug nodes

**Q5** (DeepWalk — select all): DeepWalk embeddings can capture global information better than embeddings based on cosine similarity.

**Q6** (incorporating edge features into node embeddings): $\mathbf{h}_{v}^{k} = \sigma\left( \frac{1}{|N(v)|}\sum_{u \in N(v)} \phi(\mathbf{e}_{u,v}) \mathbf{h}_{u}^{k-1} + \mathbf{B}_{k} \mathbf{h}_{v}^{k-1} \right)$, where $\phi(\mathbf{e}_{u,v})$ is a trainable neural network that maps $\mathbf{e}_{u,v}$ to $\mathcal{R}^{d_k \times d_{k-1}}$
