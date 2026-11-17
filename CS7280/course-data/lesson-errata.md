# CS7280 Lesson Errata

> Source: found while building the lesson self-checks (2026-11-05). Each item is Claude's reading of the lesson text against its own formulas and the official answer keys. No self-check question depends on any item.

## Lesson 4

### L04-1
- **Location:** [[lesson-04-unified]], section 07, maximum degree example.
- **Source text:** "one million nodes … average degree 3 … exponential … the maximum expected degree is only about 10".
- **Issue:** the lesson's formula $k_\text{max} = k_\text{min} + \ln n / \lambda$ gives about 29 to 42 for these values.

### L04-2
- **Location:** [[lesson-04-unified]], section 05, plotting choices.
- **Source text:** linear binning is "the bin width of the histogram increases linearly with $k$".
- **Issue:** linear binning keeps the bin width constant. Logarithmic binning is the one whose width grows with $k$.

### L04-3
- **Location:** [[lesson-04-unified]], section 14, sexual-contact case study.
- **Issue:** the women's and men's exponents are said to agree within statistical uncertainty, but only the men's variance is called infinite.

## Lesson 5

### L05-1
- **Location:** [[lesson-05-unified]], section 08, 7 billion people example.
- **Source text:** the random-network diameter for 7 billion people with average degree 6 is "about 22".
- **Issue:** $\ln n / \ln \bar{k} = \ln(7 \times 10^9) / \ln 6 \approx 12.65$.

## Lesson 6

### L06-1
- **Location:** [[lesson-06-unified]], betweenness centrality.
- **Source text:** "If $s$ and $t$ are the same, we define that $n_{s,t} = 1$" and the normalization "$(n-1)(n-2)$".
- **Issue:** the self-pair rule is unclear, and $(n-1)(n-2)$ counts ordered pairs, which the undirected sum does not state.

### L06-2
- **Location:** [[lesson-06-unified]], section 10, $\tau$-core.
- **Issue:** the text does not say whether path endpoints may be members of the $\tau$-core.

## Lesson 7

### L07-1
- **Location:** [[lesson-07-unified]], section 07, modularity metric.
- **Source text:** "We divided by the total number of edges $L$".
- **Issue:** the formula divides by $2L$.

### L07-2
- **Location:** [[lesson-07-unified]], section 13, modularity resolution.
- **Issue:** the factored form of $\Delta M_{AB}$ is algebraically wrong. The threshold $\kappa_l < \sqrt{2L}$ is correct.

### L07-3
- **Location:** [[lesson-07-unified]], sections 15 and 16.
- **Issue:** section 15 gives $C(k) \approx 2/k$, while section 16 gives $C(k) = 1/k$.

### L07-4
- **Location:** [[lesson07-quiz-answers]], Q6.
- **Issue:** the key "Merging communities B and D" is ambiguous for the given network.

## Lesson 8

### L08-1
- **Location:** [[lesson-08-unified]], sections 05 and 09.
- **Issue:** the $\mu$ cutoff for losing community structure is "greater than 0.5" in section 05 but "close to 1" in section 09.

### L08-2
- **Location:** [[lesson-08-unified]], participation coefficient.
- **Source text:** uniformly spread connections give a participation coefficient "close to 1".
- **Issue:** the value is exactly $1 - 1/n_c$.

### L08-3
- **Location:** [[lesson-08-unified]], run-time comparison.
- **Issue:** the text says seven algorithms, but the table lists 8.

## Lesson 9

### L09-1
- **Location:** [[lesson-09-unified]], sections 13 and 14.
- **Issue:** section 13 defines $\lambda = \beta/(\beta+\mu)$, but the SIR threshold in the section 14 table comes from Barabási, where $\lambda = \beta/\mu$.

## Lesson 10

### L10-1
- **Location:** [[lesson-10-unified]], sections 04 and 12.
- **Issue:** the threshold rule is strict in section 04 and "at least" in section 12.

### L10-2
- **Location:** [[lesson-10-unified]].
- **Issue:** the same model is named "Independent Contagion" and "Independent Cascade".

### L10-3
- **Location:** [[lesson-10-unified]], ALT model validation transcript.
- **Source text:** agreement "varies between 55 to 8%".
- **Issue:** the upper value appears truncated in the transcript.

### L10-4
- **Location:** [[lesson-10-unified]], dense clusters example.
- **Issue:** "θ larger than 2/3" depends on a figure that the text does not reproduce.

## Lesson 11

### L11-1
- **Location:** [[lesson-11-unified]], Kuramoto model.
- **Source text:** $K_c = 2/(\pi \Omega)$.
- **Issue:** Claude believes the standard result uses the frequency density $g(\Omega)$ at its center, not the mean frequency. The text also does not say whether $K$ or $K/\bar{k}$ is compared with $K_c$.

## Lesson 12

### L12-1
- **Location:** [[lesson-12-unified]], maximum likelihood of HRG probabilities.
- **Issue:** the dendrogram likelihoods 0.00165 and 0.0433 depend on a figure that the text does not reproduce.

## Lesson 13

### L13-1
- **Location:** [[lesson13-quiz-answers]], Q6.3.
- **Issue:** the key conflicts with section 11, which calls traffic matrix inference a tomography problem.

### L13-2
- **Location:** [[lesson13-knowledge-check-answers]], Q2.4.
- **Issue:** the key is debatable when $\rho_s \rho_t b$ is small.

### L13-3
- **Location:** [[lesson-13-unified]], star sampling.
- **Source text:** $\bar{k}_\text{star-sampling} = 2|E^*|/n$.
- **Issue:** the result does not match $\sum k_i / n$ over the sampled nodes.

### L13-4
- **Location:** [[lesson13-quiz-answers]], Q5.2.
- **Issue:** the key conflicts with the lesson's statement about the Fisher transformation's variance.

## Lesson 14

### L14-1
- **Location:** [[lesson-14-unified]], GNN training and decoders.
- **Issue:** the output $\sigma(\mathbf{z}_v^T \mathbf{D})$ is a sigmoid but is called "softmax".

### L14-2
- **Location:** [[lesson14-quiz-answers]], Q4.3.
- **Issue:** the key marks True for "increases with the number of nodes used in training".
