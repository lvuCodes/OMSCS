---
Title: Assignment 3
Course: Network Science - CS-7280-O01
Points: 100
Available: 22 Jun 2026, 7:00 – 9 Jul 2026, 7:00
Due: 6 Jul 2026, 7:00
Submission: External tool (Gradescope)
---

# Assignment 3

Download: [assignment_3.zip](https://gatech.instructure.com/courses/552990/files/74874949/download?download_frd=1)

In the zip file above you will find:

- **A3.ipynb**: a Jupyter notebook (.ipynb) file
- **data/**: a directory called 'data' with one or more files

## Instructions

To complete this assignment, follow the steps below:

1. Extract the contents into a local working directory (which we'll refer to as LWD) on your machine.
2. Open your Conda CLI and navigate to your LWD.
3. Open Jupyter from the Conda CLI (a Jupyter interface should open in your default browser).
4. Within the Jupyter interface, open the Jupyter notebook (.ipynb) file and follow the instructions provided there. **Instructions about environment setup will be included in the notebook and must be strictly followed to run appropriately in Gradescope.**
5. **When you have completed all the work possible/desired:**
   - **Delete any cells that you added that were not already part of the notebook (such as testing cells). Additionally, remove any print statements that were not already part of the notebook or ones you weren't instructed to include in your implementation. Extra cells and print statements can sometimes trip up the autograder in Gradescope.**
   - **Run and rerun your entire notebook several times to make sure that there are no fatal errors such as improper syntax, etc.**
   - **Make sure that your entire notebook runs in a reasonable amount of time (Gradescope has a 10 minute maximum so ideally you should aim for a faster runtime locally) and avoids excessive memory usage (submissions that exceed Gradescope's memory limit can fail to run or will receive deductions).**
6. When you have completed all the notebook instructions:
   - Save a copy of the notebook as `X-A3.ipynb`, where X is your Georgia Tech username (for example, George Burdell would submit a file named `gburdell123-A3.ipynb`).
   - Submit **only your notebook** to Assignment 3 in Gradescope.
   - Ensure that your notebook runs properly in Gradescope. A visible test case will indicate whether your submission was successfully executed and graded. Please note that a successful run does **not** imply that your code is free of errors.
   - By default, Gradescope will activate the latest submission to be graded. **If you would like some other submission to be used in grading, make sure it is activated.**
7. Please note the following while working on the assignment:
   - **There are unlimited submissions.**
   - **Local testing is strongly encouraged. Sanity checks are included for some parts of the assignment.**
   - **Do not modify imports, metatags, and provided utility functions as this can cause further issues with our autograder in Gradescope.**

## Submission

Please save a copy of the notebook as `X-A3.ipynb`, where X is your Georgia Tech username (for example, George Burdell would submit a file named `gburdell123-A3.ipynb`), and upload the file to Assignment 3 on Gradescope.

## Notebook Structure

The following part breakdown, point values, and function signatures are sourced from `A3.ipynb`, not the Canvas assignment page. The conceptual background is in [assignment3-concepts.md](notes/assignment3-concepts.md) and per-function pointers are in [assignment3-helper.md](notes/assignment3-helper.md).

All code must be written between the `####IMPLEMENTATION STARTS HERE####` and `####IMPLEMENTATION ENDS HERE####` markers. Do not add additional cells; remove any helper/testing functions before submitting.

### Part 1 — [30 pts] Centrality Metrics and Jaccard Similarity

- **1.1 [4 pts] Spectral radius** — `compute_lambda(G)`
- **1.2 [10 pts] Seven centralities (weighted then unweighted)** — `get_centralities(G, alpha)`
- **1.3 [6 pts] Top-n node sets** — `top_nodes(G, n)`
- **1.4 [7 pts] Pairwise Jaccard similarity matrix** — `get_similarity_matrix_centrality(G, n)`
- **1.5 [3 pts] Conceptualization** — three `response_*` functions

### Part 2 — [30 pts] Community Detection and NMI Similarity

- **2.1 [4 pts] Community partitions (four algorithms)** — `get_community_partitions(G, k, resolution)`
- **2.2 [10 pts] Partitions to per-node labels** — `get_community_labels(G, k, resolution)`
- **2.3 [8 pts] Pairwise NMI similarity matrix** — `get_similarity_matrix_comm_detect(G, k, resolution)`
- **2.4 [6 pts] Extended matrix with ground-truth row/column** — `get_extended_sim_mat_comm_detect(...)`
- **2.5 [2 pts] Similarity to ground truth** — one `response_*` function

### Part 3 — [10 pts] Network Centralization (Freeman)

- **3.1 [6 pts] Freeman centralization values** — `get_centralization_values(G)`
- **3.2–3.4 [1 pt each] Node centrality vs. centralization** — one `response_*` function each (betweenness, closeness, degree)
- **3.5 [1 pt] Empirical comparison** — `load_empirical_graphs()` plus `response_*` functions

### Part 4 — [30 pts] Benchmarking with LFR Networks

- **4.1 [14 pts] LFR network and ground-truth labels** — `generate_lfr_network_and_labels(mu, ...)`
- **4.2 [8 pts] Sweep over the mixing parameter** — `sweep_of_lfr_networks_over_mu(network_ct)`
- **4.3 [6 pts] NMI across the sweep** — `get_nmi_for_sweep(...)`
- **4.4 [2 pts] Algorithm performance** — one `response_*` function
