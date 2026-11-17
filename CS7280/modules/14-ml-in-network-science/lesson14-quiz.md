# Lesson 14 — Quiz (graded)

> Source: Canvas — CS-7280-O01, OAN (Summer 2026)

Combined view of the six graded quiz questions. For multiple true/false questions, consider each item as its own separate, independent statement. See also [[lesson14-quiz-all.pdf]].

---

### Q1 — Fill in the Blank (1 point)

Consider node embedding methods that are based on fixed-length random-walks, such as node2vec or DeepWalk. Which of the following statements is/are true:

1. To apply these methods we first need to calculate analytically the conditional probability of visiting a node $v$ on a length-$T$ random-walk that starts at node $u$ (where $T$ is a given positive integer). — `True` / `False`
2. The conditional probabilities mentioned in (1) are computed numerically, by simulating a number of random walks of length-$T$ from each node $u$. — `True` / `False`
3. The softmax function is the only formula that can express the previous conditional probabilities correctly. — `True` / `False`
4. If the length $T$ of the random walks is equal to one hop, the random-walk based method becomes asymptotically (for a very large sample of random walks) equivalent with the adjacency-based node embedding methods. — `True` / `False`

---

### Q2 — Multiple choice (1 point)

Suppose that you know that the nodes of a social network can be classified as follows: computer science majors, math majors, and engineering majors. You only have one labeled node for each of the three classes — but you also know that students tend to make social connections with students of the same major. Which of the following approaches do you expect would perform best in this classification problem?

- [ ] Classify each node based on the minimum shortest-path length between that node and the three labeled nodes.
- [ ] Compute adjacency-based node embeddings, and classify each node based on the shortest distance between its embedding vector and the embedding vectors of the three labeled nodes.
- [ ] Compute random-walk node embeddings (with a length that is more than 1 but much less than the network diameter), and classify each node based on the shortest distance between its embedding vector and the embedding vectors of the three labeled nodes.
- [ ] Use a supervised learning approach to train a deep graph neural network using the three labeled nodes.

---

### Q3 — Fill in the Blank (1 point)

Consider the GNN we reviewed in the polypharmacy application. Which of the following statements is/are true?

1. To compute the embedding of a drug-node $v$ at a certain layer of the GNN we need a different matrix of parameters for each neighbor of $v$. — `True` / `False`
2. To compute the embedding of a drug-node $v$ at a certain layer we need a different matrix of parameters for each type of edge that $v$ connects to. — `True` / `False`
3. We cannot compute the embedding of a drug-node $v$ at layer-$k$ if we do not know the target proteins of $v$. — `True` / `False`
4. Suppose that we know the target proteins of a drug $v$ — but we do not know any side-effects caused by the interaction of $v$ with other drugs. We can still compute the embedding of $v$. — `True` / `False`

---

### Q4 — Fill in the Blank (1 point)

GNNs have inductive ability, in the sense that we can compute embeddings even for nodes that we do not use in the training process. Which of the following statements is/are correct?

1. This inductive ability is feasible because we use the same trainable parameters for all nodes. — `True` / `False`
2. This inductive ability assumes that the nodes we use in the training process have the same statistical properties with the rest of the nodes. — `True` / `False`
3. This inductive ability increases with the number of nodes we use in the training process. — `True` / `False`
4. This inductive ability can also be used to compute the embeddings of future nodes that are added to the network after the training process. — `True` / `False`

---

### Q5 — Fill in the Blank (1 point)

Suppose you want to use a GNN to classify the nodes of a social network (for example, the classes may be: "Democrat", "Republican", "Undecided", "Other"). Suppose that you know the correct label (i.e., the political affiliation) for some of the nodes. Additionally, you know some additional attributes (gender, age, education level) for all nodes. Which of the following statements is/are correct?

1. The initial layer-0 embeddings are equal to the node features. — `True` / `False`
2. A layer-3 node embedding depends on the layer-2 node embeddings of that node's neighbors. — `True` / `False`
3. The training data should consist of all nodes for which we know the political affiliation. — `True` / `False`
4. The larger the number of layers (depth) of the network, the more susceptive the network is to overfitting. — `True` / `False`

---

### Q6 — Multiple choice (1 point)

The question concerns the "minimum temporal spanning tree" concept introduced in this lesson. The following figure shows the communications between six nodes, arranged temporally in 4 time steps. Node-A has some information initially that it wants to share with the rest of the nodes. Which of the following is the "minimum temporal spanning tree" originating at node-A?

![[img/quiz-q06-timeline.png|500]]

- [ ] ![[img/quiz-q06-option-1.png|300]]
- [ ] ![[img/quiz-q06-option-2.png|300]]
- [ ] ![[img/quiz-q06-option-3.png|300]]
- [ ] ![[img/quiz-q06-option-4.png|300]]
