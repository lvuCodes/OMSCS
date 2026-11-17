# CSE 6220 Course Readiness Survey

Source: [omscs.gatech.edu/sites/.../CSE 6220-Course Readiness Survey.pdf](https://omscs.gatech.edu/sites/default/files/documents/2023/CSE%206220-Course%20Readiness%20Survey.pdf) (image-only PDF, transcribed; retained as [readiness-survey.pdf](readiness-survey.pdf)).

## Questions

1. **Big-Oh my!** You have been asked to choose one of two possible algorithms. You are given just two facts. First, one algorithm has an asymptotic running time of $O(n^{1.1})$ and the other $O(n \log_2 n)$. Secondly, $n$ will be really huge. Which would you choose and why?

2. **Probability.** Suppose you roll a pair of 6-sided dice. What is the probability that the sum of pairs' values will be even?

3. **Calculus.** Consider the following function:

   $$\Gamma(a) = \int_0^\infty t^{a-1} e^{-t}\, dt.$$

   Show that $\Gamma(a) = (a-1)\,\Gamma(a-1)$.

4. **Algorithms and data structures.** Consider an undirected graph $G = (V, E)$, where $V$ is the set of its vertices and $E$ its edges. We say $G$ is *bipartite* if there exists a partitioning of the vertices, $V = V_1 \cup V_2$, such that

   a. $V_1 \cap V_2 = \emptyset$, that is, $V_1$ and $V_2$ are disjoint; and
   b. for every edge $(u, v) \in E$, $u \in V_1$ and $v \in V_2$ or $v \in V_1$ and $u \in V_2$. That is, all edges go between $V_1$ and $V_2$, and no edges lie wholly within a single partition.

   Give an algorithm to check whether a graph is bipartite.

## Suggested Background (course page)

The OMSCS course page lists the expected preparation:

- CS 6515 (Intro to Graduate Algorithms) or an undergraduate algorithms course
- Programming experience in C or C++
- Command-line proficiency in Unix/Linux
