# Lesson 10 — Quiz Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results (7/7, 100%)

Questions: [[lesson10-quiz]].

---

**Q1** (node to activate in addition to 1 and 8, linear threshold $0.6$): **2**

**Q2** (unpaired-socks function $f(S)$):
1. False — The function is monotone
2. True — $f(\emptyset) = f(U) = 0$
3. True — The function is submodular
4. True — The function's maximum value is dependent on $|U|$

**Q3** (statement NOT true in general for monotone submodular cascade size): The nodes that will become active after activating $v$ may include some nodes that make up $f(S)$ but do not make up $f(T)$

**Q4** (communities and cascade sizes, homogeneous linear threshold $\theta$):
1. False — The cascade can reach the entire network only if the linear threshold is less than the lowest community density
2. False — The cascade can reach the entire network only if the initial active set includes a node in each community
3. True — The cascade cannot reach the members of a community if the density of that community is greater than $1 - \theta$
4. False — The cascade cannot reach the members of a community if the density of that community is greater than $\theta$

**Q5** (asynchronous linear threshold model):
1. False — Initializing from the $k$ highest out-strength nodes always leads to a larger cascade than $k$ random nodes
2. False — The time delays can change which nodes end up being active after the cascade completes
3. True — This model allows us to create a DAG representing the order in which nodes become activated
4. False — The total time units required equals the depth of the cascade

**Q6** (why Shadi et al. used the ALT model): So that they can compare the timing of the cascade according to the model with experimental results

**Q7** (coordination game, $b > c$): The maximum cumulative "payoff" across all nodes in the network is $2M(b-c)$, where $M$ is the total number of edges in the network
