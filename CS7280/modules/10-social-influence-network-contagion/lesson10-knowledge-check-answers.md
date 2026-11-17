# Lesson 10 — Knowledge Check Answer Key

> Source: Canvas — CS-7280-O01, OAN (Summer 2026) — graded results

Questions: [[lesson10-knowledge-check]].

---

**Q1** (Linear Threshold cascade with threshold 0.6): **Option 4**

**Q2** (Deffuant convergence parameter $\mu$ that flips neighboring opinions every iteration): $\mu = 1.0$

**Q3** (menu-bundle pricing function): The function is monotone

**Q4** (nodes activated only after adding $v$ to the initial active set):
1. False — Some of them may belong to the original cascade of $S$ but not to the original cascade of $T$.
2. True — Some of them may belong to neither the initial cascade of $S$, nor the initial cascade of $T$.
3. True — Some of them may belong to the initial cascade of $T$ but not to the initial cascade of $S$.
4. False — Some of them may belong to both the initial cascade of $S$ and of $T$.

**Q5** (activating an entire community whose density exceeds $1-\theta$): Include a fraction of community members greater than $\theta$ in the initially activated set.

**Q6** (linear threshold vs. SIS):
1. True — In the SIS model a node can become susceptible again, but in the linear threshold model once a node has become activated it stays that way.
2. True — With a given initially active set of nodes, the linear threshold model is deterministic while the SIS model is probabilistic.
3. False — The linear threshold model can lead to oscillating dynamics while the SIS model cannot.
4. True — Both models may lead to complete cascades/epidemics, activating (or infecting, respectively) all nodes of the network.

**Q7** ($\min(f(X), g(X))$ and $\max(f(X), g(X))$ for submodular $f$ and $g$): The two functions may not be submodular
