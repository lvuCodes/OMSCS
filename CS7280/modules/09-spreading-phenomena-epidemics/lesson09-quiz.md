# Lesson 9 — Quiz (graded)

> Source: Canvas — CS-7280-O01, OAN (Summer 2026)

Combined view of the six graded quiz questions. See also [[lesson09-quiz-all.pdf]]. The answer key is in [[lesson09-quiz-answers]].

---

### Q1 — Fill in the Blank (1 point)

In the case of the SIS model, the ratio of $\frac{\bar{k}\beta}{\mu}$ is critical for defining the outcome of the outbreak. Which of the following are true about the outcome of an outbreak given specific ratio of $\frac{\bar{k}\beta}{\mu}$?

1. When $\bar{k}\beta > \mu$ and for small values of $t$, the solution to the SIS model can be approximated as $i(t) \approx i_0 e^{(\bar{k}\beta - \mu)t}$. — `True` / `False`
2. When $\bar{k}\beta < \mu$ the number of new infections decreases exponentially from $i_0$ to $1 - \frac{\bar{k}\beta}{\mu}$. — `True` / `False`
3. When $\bar{k}\beta < \mu$ the number of new infections decreases exponentially from $i_0$ to $0$. — `True` / `False`
4. When $\bar{k}\beta > \mu$ the percentage of the population that is infected will converge to a value that depends on $i_0$. — `True` / `False`

---

### Q2 — Multiple choice (1 point)

In networks with scale-free degree distributions and exponent $\gamma$, if $2 < \gamma < 3$ then the variance (and the second moment) of the degree diverges to infinity. What does this mean in terms of the conditions for an epidemic?

- [ ] Everyone gets infected
- [ ] Outbreaks in networks with scale-free degree distributions ($2 < \gamma < 3$) always lead to an epidemic.
- [ ] The value of $\beta$ and $\mu$ are no longer included in the expression for the steady state fraction of infected individuals.
- [ ] When $2 < \gamma < 3$ the dynamics of scale free networks are exactly the same as random networks

---

### Q3 — Fill in the Blank (1 point)

Which of the following are true about the homogeneous mixing assumption in epidemic models?

1. It assumes that the number of contacts of each individual is random — `True` / `False`
2. It is appropriate when we do not need to know the exact contact network between individuals — `True` / `False`
3. It assumes that the number of contacts is the same for each individual — `True` / `False`
4. It assumes that the number of contacts follows a power-law distribution — `True` / `False`

---

### Q4 — Multiple choice (1 point)

What information is NOT captured by $R_0$ even though it has a major impact on the actual spread of an epidemic?

- [ ] The variance in the attack rate across individuals
- [ ] The variance in the number of contacts across individuals
- [ ] The variance in the resistance to infection between individuals
- [ ] All of the above

---

### Q5 — Multiple choice (1 point)

Under the SIS model with an arbitrary degree distribution, it was shown that $\theta_k(t)$ does not depend on $k$. Why is this important?

- [ ] It tells us that the probability that your neighbor is infected is not related to his/her degree
- [ ] It tells us that the probability that your neighbor is infected is unrelated to your degree
- [ ] It tells us that the probability that your neighbor is infected is unrelated to the degree distribution
- [ ] It is just a notational simplification

---

### Q6 — Multiple choice (1 point)

Which of the following has been observed in practice using human mobility data and computational modeling of epidemics?

- [ ] There is a strong correlation between the time it takes for a pandemic to reach a certain location and the geographic distance between that location and the origin of the epidemic
- [ ] There is a strong correlation between the time it takes for a pandemic to reach a certain location and the effective distance between that location and the origin of the epidemic
- [ ] The effective distance calculation depends on the specific pathogen
- [ ] The effective distance between two locations $i$ and $j$ is given by $1 - p_{i,j}$
