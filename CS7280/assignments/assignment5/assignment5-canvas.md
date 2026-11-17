---
Title: Assignment 5
Course: Network Science - CS-7280-O01
Points: 100
Available: 20 Jul 2026, 7:00 – 6 Aug 2026, 7:00
Due: 3 Aug 2026, 7:00
Submission: External tool (Gradescope)
---

# Assignment 5 — Network Modeling, Statistics, and Machine Learning

Download: [assignment_5.zip](https://gatech.instructure.com/courses/552990/files/75376479/download?download_frd=1)

In the zip file above you will find:

- **A5.ipynb**: a Jupyter notebook (.ipynb) file
- **data/**: a directory called 'data' with one or more files (`football.gml`, `football-hrg.gml`, `mouse_brain_data.txt`)
- **environment.yml**: a file with module dependencies, for reference only (generated on a Windows machine)
- **nlp_data.py**: a module holding the data used for the machine-learning parts (Parts 4 and 5); no install needed
- **PyHRG/**: a bundled partial implementation of [Hierarchical Random Graphs](http://tuvalu.santafe.edu/~aaronc/hierarchy/), used to pre-compose the `data/football-hrg.gml` dendrogram; reference only, not imported by the notebook

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
   - Save a copy of the notebook as `X-A5.ipynb`, where X is your Georgia Tech username (for example, George Burdell would submit a file named `gburdell123-A5.ipynb`).
   - Submit **only your notebook** to Assignment 5 in Gradescope.
   - Ensure that your notebook runs properly in Gradescope. A visible test case will indicate whether your submission was successfully executed and graded. Please note that a successful run does **not** imply that your code is free of errors.
   - By default, Gradescope will activate the latest submission to be graded. **If you would like some other submission to be used in grading, make sure it is activated.**
7. Please note the following while working on the assignment:
   - **There are unlimited submissions.**
   - **Local testing is strongly encouraged. Sanity checks are included for some parts of the assignment.**
   - **Do not modify imports, metatags, and provided utility functions as this can cause further issues with our autograder in Gradescope.**

## Submission

Please save a copy of the notebook as `X-A5.ipynb`, where X is your Georgia Tech username (for example, George Burdell would submit a file named `gburdell123-A5.ipynb`), and upload the file to Assignment 5 on Gradescope.

## Environment Note

Assignment 5 introduces three dependencies not present in A1–A4: [ridgeplot](https://pypi.org/project/ridgeplot/) (`ridgeplot==0.3.2`), [PyTorch](https://pytorch.org/) (`torch==2.5.1`), and [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/) (`torch-geometric==2.6.1`), alongside `seaborn` (bumped to `0.13.2`). The shipped `environment.yml` is a Conda/Python-3.10 spec generated on Windows and is reference-only; this local environment is a pyenv-managed Python 3.11.9 `.venv` built from [requirements.txt](assignment_5/requirements.txt) and pinned in [requirements.lock.txt](assignment_5/requirements.lock.txt). The NLP data ships as `nlp_data.py` (imported inside the notebook as `nlp_data`); there is no external `test_a5.py` harness.

## Notebook Structure

The following part breakdown, point values, and function signatures are sourced from `A5.ipynb`, not the Canvas assignment page. The assignment spans Modules 12–14: structural community analysis, three network-generation algorithms, sampling-based network estimation, and two natural-language-processing approaches (label propagation and a Graph Attention Network).

All code must be written between the `####IMPLEMENTATION STARTS HERE####` and `####IMPLEMENTATION ENDS HERE####` markers. Do not add additional cells; any extra helper functions must be nested or inline inside the existing marked region, and cell tags (`export`, `test`) must be preserved.

**Part connections:** Part 2 calls some of the functions from Part 1. Parts 4 and 5 are conceptually linked — either can be done independently, but Part 4's pedagogical throughline carries into Part 5.

### Part 1 — [20 pts] Structural Properties of Networks (Module 12)

Provided (run, do not modify): `load_football_network` (115 nodes, 613 edges), `util_community_labels`, `util_ground_truth_community_labels`, and plotters (`util_plot_nmi_vs_resolution`, `util_plot_best_partition`, `util_plot_p_matrix`).

- **1.1 [4 pts] Descriptive graph statistics** — `calculate_graph_statistics(G)`
- **1.2 [4 pts] Community assignments and NMI** — `sweep_louvain_resolutions(G, ...)`
- **1.3 [4 pts] Optimize Louvain resolution based on NMI** — `calculate_best_partition(G, ...)`
- **1.4 [4 pts] Inter-community density** — `calculate_inter_community_density(G, partition)`
- **1.5 [0 pts] Visualization** — provided plotting cell
- **1.6 [4 pts] Analysis** — `part_1_analysis_q1_response()`, `part_1_analysis_q2_response()`

### Part 2 — [35 pts] Network Generation (Module 12)

- **2.1 [7 pts] Configuration graph** — `generate_configuration_graphs(degree_sequence, n_graphs=100)`
- **2.2 [7 pts] Stochastic Block Model** — `generate_sbm_graphs(p, sizes, n_graphs=100)`
- **2.3 [7 pts] Hierarchical Random Graph** — `calculate_edge_probability(dendrogram)`, `generate_graph_from_prob(edge_probs)`, `generate_hrg_graphs(edge_probs, n_graphs=100)` (with provided `util_get_root`, `util_get_lowest_parent`); dendrogram loaded from `data/football-hrg.gml`
- **2.4 [7 pts] Network statistics** — `calculate_generated_statistics(graphs)` (with provided `util_get_LCC`)
- **2.5 [0 pts] Visualization** — `util_plot_graph_statistics`
- **2.6 [7 pts] Analysis** — `part_2_analysis_q1_response()`, `part_2_analysis_q2_response()`

### Part 3 — [25 pts] Network Estimation (Module 13)

Provided: `load_mouse_brain_network` (213 nodes, 16,242 edges).

- **3.1 [9 pts] Estimate node count** — `estimate_network_size(G, sample_sizes=[5,10,50,100], n_iter=100)`
- **3.2 [9 pts] Estimate edge count** — `estimate_edges(G, n_sample=50, n_iter=100)`
- **3.3 [0 pts] Visualizations** — `util_plot_histos_as_ridge`, `util_plot_sample_size_error`
- **3.4 [7 pts] Analysis** — `part_3_analysis_q1_response()`, `part_3_analysis_q2_response()`

### Part 4 — [10 pts] NLP Using Label Propagation (Module 14)

- **4.1 [1 pts] Corpus network** — `get_corpus_network()`
- **4.2 [1 pts] Biadjacency matrix of corpus network** — `get_corpus_biadjacency_matrix(text_data)`
- **4.3 [1 pts] Get text data and labels** — `get_training_text_and_labels(perc_of_corpus=0.5)`
- **4.4 [1 pts] Scrubbing labels** — `scrub_labels(perc_unscrubbed=0.1, labels_true=[])`
- **4.5 [1 pts] Training label propagation model** — `get_trained_label_prop_model(text_data, labels_scrubbed)`
- **4.6 [2 pts] Model accuracy** — `get_accuracy(label_prop_model, text_data, labels_true, show)`
- **4.7 [2 pts] Putting it all together** — `run_full_label_prop(...)`
- **4.8 [0 pts] Visualization** — `util_show_label_prop_accuracy`
- **4.9 [1 pts] Analysis** — `part_4_analysis_q1_response()`

### Part 5 — [10 pts] NLP Using a Graph Attention Network (GAT) (Module 14)

Two framings: **vA** — a single large, sparse network; **vB** — many small networks plus one moderately-sized, highly connected network.

- **5.1 [2 pts] Tokenization** — `get_sentence_tokenized(sentence)`, `get_tokenized_sentences_and_labels()`
- **5.2 [1 pts] Word embeddings** — `get_word_vec(word, word2idx, embedding)` (with provided `util_get_word_embedding`, `util_show_word_embedding_2d`)
- **5.3 [1 pts] Node features** — `part_5_node_feature_q_response()` (with provided `util_show_word_embedding_as_features`)
- **5.4 [3 pts] Message passing pt 1** — `get_sentence_idx_graph(...)`, `message_pass_on_embedding_matrix(...)` (with provided `util_show_message_passing`)
- **5.5 [1 pts] Message passing pt 2** — `part_5_message_passing_q_response()`
- **5.6 [1 pts] Pooling node features to a graph-level label** — `get_global_average_pooling(...)`
- **5.7 [0 pts] Training a GAT network** — provided `util_get_train_test_split`, `util_get_trained_GAT`
- **5.8 [0 pts] Experiments** — provided run cell (tune `EPOCHS`, `LR`, `TEST_SIZE` only)
- **5.9 [1 pts] Analysis** — `part_5_q1_response()`
