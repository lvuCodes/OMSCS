# Lesson 10 — Quiz (graded)

> Source: Canvas — CS-7280-O01, OAN (Summer 2026)

Combined view of the seven graded quiz questions. For multiple true/false questions, consider each item as its own separate, independent statement. See also [[lesson10-quiz-all.pdf]]. The answer key is in [[lesson10-quiz-answers]].

---

### Q1 — Multiple choice (1 point)

Given this graph and a linear threshold of $0.6$ (activation condition for nodes is $\geq$), which node would you select to activate in addition to nodes 1 and 8 so that all nodes become active eventually?

![[img/quiz-q01-graph.png|500]]

- [ ] 2
- [ ] 10
- [ ] 3
- [ ] 5

---

### Q2 — Fill in the Blank (1 point)

Consider that we have a number of pairs of socks (assuming that they are all unique pairs). Let $U$ be the set of all individual socks. Let $S$ be a subset of $U$. Define $f(S)$ as the number of unpaired socks in $S$. Which of the following statements are TRUE about $f(S)$?

1. The function is monotone. — `True` / `False`
2. $f(\emptyset) = f(U) = 0$. — `True` / `False`
3. The function is submodular. — `True` / `False`
4. The function's maximum value is dependent on $|U|$ — the cardinality of $U$. — `True` / `False`

---

### Q3 — Multiple choice (1 point)

We have seen that the cascade size function with the Independent Cascade model is monotone and submodular. Consider two sets of initially active nodes $S$ and $T$, where $S \subset T$. The function $f(X)$ maps from a set of active nodes $X$ to the size of the resulting cascade. Which of the following statements is NOT true in general?

- [ ] The nodes that will become active after activating $v$ may include some nodes that make up $f(S)$ but do not make up $f(T)$.
- [ ] The cascade size of both $S$ and $T$ may increase by the same amount.
- [ ] The nodes that will become active after activating $v$ may only include $v$.
- [ ] The nodes that will become active after activating $v$ may increase the cascade size of $S$ more than the cascade size of $T$.

---

### Q4 — Fill in the Blank (1 point)

Which of the following is true about communities and cascade sizes in networks with a homogeneous linear threshold model (assume that the threshold is $\theta$)?

1. The cascade can reach the entire network only if the linear threshold is less than the lowest community density in the network. — `True` / `False`
2. The cascade can reach the entire network only if the initial set of active nodes includes a node in each community. — `True` / `False`
3. The nodes of the network are inactive except for the initial set of active nodes. The resulting cascade cannot reach the members of a community if the density of that community is greater than $1 - \theta$. — `True` / `False`
4. The nodes of the network are inactive except for the initial set of active nodes. The resulting cascade cannot reach the members of a community if the density of that community is greater than $\theta$. — `True` / `False`

---

### Q5 — Fill in the Blank (1 point)

Which of the following is/are true about cascades under the asynchronous linear threshold model?

1. Initializing the cascade from the set of $k$ nodes with the highest out-strength (sum of weights of outgoing edges) will always lead to a larger cascade than initializing the cascade from $k$ randomly chosen nodes. — `True` / `False`
2. The time delays can change which nodes end up being active after the cascade has completed. — `True` / `False`
3. This model allows us to create a DAG to represent the order in which nodes become activated in the cascade. — `True` / `False`
4. The total time units required for the cascade to propagate through the network is equal to the depth of the cascade. — `True` / `False`

---

### Q6 — Multiple choice (1 point)

In the study by Shadi et al. about multi-sensory integration in the mouse brain, the authors use the ALT model. Why did those authors choose to use the Asynchronous Linear Threshold model instead of the Linear Threshold model? (the latter does not consider link delays)

- [ ] Link delays make the model more robust to the selection of the activation threshold
- [ ] So that they can compare the timing of the cascade according to the model with experimental results
- [ ] Without link delays, they would not get the right cascades
- [ ] Without link delays, it would not be possible to identify the central nodes that are responsible for multi-sensory integration

---

### Q7 — Multiple choice (1 point)

Based on the network and coordination game rule ($b > c$) in the following figure, which of the following statements is TRUE?

![[img/quiz-q07-figure.png|500]]

- [ ] The maximum cumulative "payoff" across all nodes in the network is reached when every node chooses the strategy that it would benefit itself at the next step.
- [ ] The maximum cumulative "payoff" across all nodes in the network is $2M(b-c)$, where $M$ is the total number of edges in the network.
- [ ] If the neighbors of node $v$ ($x, y, w, u$) are all cooperators, the "payoff" that $v$ gets does not depend on $v$'s strategy.
- [ ] The highest "payoff" for $v$ is $4b - 4c$.
