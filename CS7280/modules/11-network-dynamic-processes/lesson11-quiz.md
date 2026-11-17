# Lesson 11 — Quiz (graded)

> Source: Canvas — CS-7280-O01, OAN (Summer 2026)

Combined view of the seven graded quiz questions. For multiple true/false questions, consider each item as its own separate, independent statement. See also [[lesson11-quiz-all.pdf]]. The answer key is in [[lesson11-quiz-answers]].

---

### Q1 — Fill in the Blank (1 point)

Which of the following statement is TRUE?

1. For a power-law network under random failures, the critical threshold $f_c$ decreases as $\gamma$ increases. — `True` / `False`
2. The Molloy-Reed criterion is applicable to any network. — `True` / `False`
3. Power-law networks disintegrate into multiple components after removing only a few random nodes. — `True` / `False`
4. Random removal of a fraction of nodes causes a larger decrease in the size of the giant component than random removal of the same fraction of edges. — `True` / `False`

---

### Q2 — Fill in the Blank (1 point)

Which of the following statements are TRUE regarding a power-law network with degree exponent $\gamma$, minimum degree $k_{min}$, and a corresponding critical threshold $f_c$?

1. In the case of attacks, $f_c$ for $k_{min}=3$ is less than $f_c$ for $k_{min}=2$. — `True` / `False`
2. In the case of random failures, $f_c$ increases as $\gamma$ increases. — `True` / `False`
3. In the case of attacks, for $k_{min}=3$, $f_c$ increases as $\gamma$ increases. — `True` / `False`
4. For the same value of $k_{min}$, the critical threshold for random failures and the critical threshold for attacks become asymptotically equal as $\gamma$ increases. — `True` / `False`

---

### Q3 — Multiple choice (1 point)

In Kleinberg's model, for a 3-dimensional grid, if we have an exponent $q = 2$, how are the long-range links distributed?

- [ ] There will be a large fraction of links covering long distances
- [ ] The links are uniformly distributed over all resolution scales
- [ ] There will be a large fraction of links covering short distances
- [ ] The link distribution does not depend on exponent $q$

---

### Q4 — Multiple choice (1 point)

In the Kuramoto model, what is the critical value of the coupling strength $K_c$ that is necessary for the onset of complete synchronization?

- [ ] $\frac{2\pi}{\Omega}$
- [ ] $\frac{2}{\pi\Omega}$
- [ ] $\frac{1}{2\pi\Omega}$
- [ ] $\frac{1}{\pi\Omega}$

---

### Q5 — Fill in the Blank (1 point)

In the context of consensus formation in adaptive networks, which of the following are TRUE?

1. In an adaptive network, global consensus is harder to reach for high tolerance values. — `True` / `False`
2. When the tolerance value is low, smaller consensus clusters are formed in the adaptive network, compared to the static network. — `True` / `False`
3. Global consensus is easier to achieve in the adaptive network. — `True` / `False`
4. Large consensus clusters are obtained even at low tolerance in adaptive networks. — `True` / `False`

---

### Q6 — Multiple choice (1 point)

Consider the following sequence of Twitter events between 4 users:

- Step 0: Joe and Ravi follow Mary. Mary follows Leila.
- Step 1: Leila sends a tweet.
- Step 2: Ravi follows Leila.
- Step 3: Mary retweets Leila's message.
- Step 4: Joe follows Leila.
- Step 5: Leila follows Joe.
- Step 6: Ravi follows Joe.

Which of these topological changes can be described as adaptive (i.e., caused by information transfer activity on the network)?

- [ ] Joe following Leila
- [ ] Ravi following Leila
- [ ] Mary following Leila
- [ ] Ravi following Joe

---

### Q7 — Fill in the Blank (1 point)

In the following figure, we show two regular networks and the position of two nodes $v$ and $w$. To maximize the speed of decentralized search in these networks, which of the following approaches should we follow?

![[img/quiz-q07-networks.png|400]]

1. For network (a), the probability of random "shortcut links" should decay with $d(v, w)^{-2}$. — `True` / `False`
2. For network (a), the probability of random "shortcut links" should decay with $rank_v(w)^{-1}$. — `True` / `False`
3. For network (b), the probability of random "shortcut links" should decay with $d(v, w)^{-2}$. — `True` / `False`
4. For network (b), the probability of random "shortcut links" should decay with $rank_v(w)^{-2}$. — `True` / `False`
