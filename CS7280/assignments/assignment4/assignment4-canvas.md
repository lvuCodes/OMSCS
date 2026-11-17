---
Title: Assignment 4
Course: Network Science - CS-7280-O01
Points: 100
Available: 6 Jul 2026, 7:00 – 23 Jul 2026, 7:00
Due: 20 Jul 2026, 7:00
Submission: External tool (Gradescope)
---

# Assignment 4 — Spreading Phenomena on Networks

Download: [assignment_4.zip](https://gatech.instructure.com/courses/552990/files/75074059/download?download_frd=1)

In the zip file above you will find:

- **A4.ipynb**: a Jupyter notebook (.ipynb) file
- **data/**: a directory called 'data' with one or more files
- **sanity_checks.py**: a file containing data used in one or more of the sanity checks

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
   - Save a copy of the notebook as `X-A4.ipynb`, where X is your Georgia Tech username (for example, George Burdell would submit a file named `gburdell123-A4.ipynb`).
   - Submit **only your notebook** to Assignment 4 in Gradescope.
   - Ensure that your notebook runs properly in Gradescope. A visible test case will indicate whether your submission was successfully executed and graded. Please note that a successful run does **not** imply that your code is free of errors.
   - By default, Gradescope will activate the latest submission to be graded. **If you would like some other submission to be used in grading, make sure it is activated.**
7. Please note the following while working on the assignment:
   - **There are unlimited submissions.**
   - **Local testing is strongly encouraged. Sanity checks are included for some parts of the assignment.**
   - **Do not modify imports, metatags, and provided utility functions as this can cause further issues with our autograder in Gradescope.**

## Submission

Please save a copy of the notebook as `X-A4.ipynb`, where X is your Georgia Tech username (for example, George Burdell would submit a file named `gburdell123-A4.ipynb`), and upload the file to Assignment 4 on Gradescope.

## Environment Note

Assignment 4 introduces a new dependency not present in A1–A3: [EoN (Epidemics on Networks)](https://epidemicsonnetworks.readthedocs.io/en/latest/index.html), installed with `pip install EoN`. It also ships `sanity_checks.py` (imported inside the notebook as `sc`), which supplies a fixed simulation run and expected values for the in-notebook sanity checks — there is no external `test_a4.py` harness.

## Notebook Structure

The following part breakdown, point values, and function signatures are sourced from `A4.ipynb`, not the Canvas assignment page. The assignment applies the Module-4 network-epidemics theory (SIS spreading, time constants, endemic sizes) to simulations on the Dublin human-contact network, comparing empirical simulation results against the theoretical formulas derived in lecture.

All code must be written between the `####IMPLEMENTATION STARTS HERE####` and `####IMPLEMENTATION ENDS HERE####` markers. Do not add additional cells; any extra helper functions must be nested or inline inside the existing marked region, and cell tags (`export`, `test`) must be preserved.

### Part 0 — Setup [0 pts]

Provided (run, do not modify): utility loaders and plotters (`util_load_dublin_contact_network`, `util_plot_outbreaks`, `util_plot_curve_fit`, `util_plot_time_constants`, `util_compare_endemic_sizes`, `util_plot_trans_rate_time_constant_curves`, `util_plot_endemic_size_trans_rate`, `plot_centrality_vs_time_constant`), the Dublin contact network (410 nodes, 2765 edges), and a notation-mapping table between CS 7280, EoN, and this notebook.

### Part 1 — [50 pts] Outbreak Modeling

- **1.1 [6 pts] Simulating outbreak** — `simulate_outbreak_tSI(G, n_iter, initial_infected_idx, tmax, trans_rate, recover_rate)`
- **1.2 [6 pts] Getting time constant from exponential fit curve** — `get_time_constant_i_stop_r2(simulation_run, I_thresh)`
- **1.3 [6 pts] Getting empirical time constants and endemic sizes** — `get_empirical_time_constants_and_endemic_sizes(...)`
- **1.4 [6 pts] Getting theoretical time constants** — `get_theoretical_time_constants(G, trans_rate, recover_rate)`
- **1.5 [6 pts] Getting theoretical endemic size** — `calculate_theoretical_endemic_size(G, trans_rate, recover_rate)`
- **1.6 [0 pts] Visualization** — provided plotting cell
- **1.7 [20 pts] Analysis** — `part_1_analysis_q1_response()`, `part_1_analysis_q2_response()`

### Part 2 — [20 pts] Transmission Rate Variation

- **2.1 [5 pts] Transmission rate sweep** — `simulate_trans_rate_sweep(...)`
- **2.2 [5 pts] Theoretical minimum transmission rate** — `get_theoretical_trans_rate_min(G, recover_rate)`
- **2.3 [0 pts] Visualization** — provided plotting cell
- **2.4 [10 pts] Analysis** — `part_2_analysis_q1_response()`, `part_2_analysis_q2_response()`

### Part 3 — [30 pts] Patient 0 Variance

- **3.1 [10 pts] Patient 0 sweep** — `sweep_patient_zero(G, tmax, trans_rate, recover_rate, I_thresh)`
- **3.2 [5 pts] Getting centralities of impactful patient-0s** — `get_centralities(G, impactful_patient_zeros)`
- **3.3 [5 pts] Linear correlation between centrality and time constant** — `calculate_pearson_correlation(time_constants, cent_dict)`
- **3.4 [0 pts] Visualize** — provided plotting cell
- **3.5 [10 pts] Analysis** — `part_3_analysis_q1_response()`, `part_3_analysis_q2_response()`
