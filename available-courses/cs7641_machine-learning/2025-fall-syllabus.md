# CS 7641: Machine Learning — Fall 2025

Source: `downloads/CS 7641 2025-3.pdf` ([omscs.gatech.edu/sites/.../CS 7641 2025-3.pdf](https://omscs.gatech.edu/sites/default/files/documents/Syllabi/CS%207641%202025-3.pdf))

## Welcome

**Instructor:** Theodore J. LaGrow (`tlagrow@gatech.edu`)

**Head TAs:** John Mansfield (`jmansfield6@gatech.edu`), Danyang Cai (`dcai38@gatech.edu`), Jake Knigge (`jwk@gatech.edu`), Jack Henderson (`jhenderson88@gatech.edu`)

**Creators of Recorded Material:** Charles Isbell, Michael Littman

## General Information

Machine Learning is a three-credit course on the study and application of the field of Machine Learning — the area of Artificial Intelligence concerned with computational artifacts that modify and improve their performance through experience, spanning both theoretical and practical issues. This class is part of a series of Machine Learning classes and presents algorithms and approaches grounded in larger systems. Topics include statistical supervised and unsupervised learning methods, optimization algorithms, and Bayesian learning methods, as well as theoretical concepts such as inductive bias, the PAC and Mistake-bound learning frameworks, the minimum description length principle, and Ockham's Razor. This term emphasizes advanced topics to bring the material closer to the state of the art. The course includes programming and practical application across a number of projects.

## Objectives

There are four primary objectives:

- Provide foundational knowledge with a broad survey of approaches and techniques in ML.
- Develop a deeper understanding of several major topics in ML.
- Develop the design and programming skills to build intelligent, adaptive artifacts.
- Develop necessary skills to communicate research and practicum in ML.

The last bullet is the core objective and separates this offering from many others: without proper and efficient communication, no amount of coding or results will matter.

## Prerequisites

The official prerequisite is an introductory course in artificial intelligence. Experience in general representational issues in AI, some AI programming, and at least some background in statistics, vector calculus, information theory, and linear algebra should be adequate. Any student who did well in an introductory AI course should be fine; most semi-modern AI courses suggest some background in machine learning techniques as well. The most important prerequisite is interest in the material. If unsure whether the class is a fit, contact the instructor or Head TAs.

## Course Resources

- **Video Lectures.** All lectures are recorded and available in two places: (1) Canvas under Modules (primary), and (2) Canvas in Ed Lessons (beta mirror). If anything is missing or out of order, default to Modules in Canvas and flag it on Ed.
- **Readings.** The textbook is *Machine Learning* by Tom Mitchell — an older but foundational text, freely available online. The pre-recorded lectures align week-to-week with the book, so a copy is imperative. Supplemental readings are provided and updated to support advanced topics throughout the semester.
- **Computing.** No high-throughput dedicated resources are needed, but [CoC clusters](https://support.cc.gatech.edu/facilities/general-access-servers) are available for programming assignments (test on the Shuttles cluster with GT username/password; no CoC account needed). Every assignment can be queued and run on a free instance of Colab if needed.
- **Web.** The class Canvas page and Ed Discussions are used for announcements.

## Statement of Academic Honesty

Students are expected to follow the university's [academic honor code](https://policylibrary.gatech.edu/student-life/academic-honor-code). Proper attribution does not absolve a writer of intellectual honesty: copying text without attribution is plagiarism, and copying too much text even with attribution betrays a lack of intellectual honesty (too many quotes of more than ~two sentences will be considered plagiarism).

Unauthorized use of any previous-semester course materials (tests, quizzes, homework, projects, videos, and any other coursework) is prohibited; using old exams is a direct violation handled per the GT Academic Honor Code. Copies of exams may not be shared outside the course, now or in the future. Any personal attacks or unacceptable language toward students or staff on any online platform are reported with a zero-tolerance policy.

## Readings and Lectures

The online lectures summarize the readings and stress important points; students are expected to critically read assigned material. Office hours are mandatory and recorded for those who cannot attend live. A nominal schedule (see the Syllabus link) paces the material as if meeting twice a week. The Fall term offers additional advanced topics recorded by the instructor each week, supplementing the ~9-year-old original material with current state-of-the-art context.

## Scoring and Grading

The final grade is determined by a reading/writing quiz, hypothesis report practice, 4 unit quizzes, 4 comprehensive reports, and a cumulative final exam.

- **Reading/Writing Quiz.** A lecture and quiz to establish formal report reading/writing skills practiced throughout the semester. Unlimited attempts until the due date. Available at the start of week 1, due end of week 2.
- **Hypothesis Report Practice.** An exercise on hypothesis interpretation and development, supplementing the Reading/Writing Quiz with feedback before the first assignment. Available end of week 1, due end of week 2.
- **Unit Quizzes.** One quiz per unit (SL, OL, UL, RL). Each unit is three weeks; the quiz opens in week 1 of the unit and is open until the end of week 3. Questions are a mix of selection and calculation drawn randomly from a test bank. 60 minutes total, 3 attempts over the window, with correct/incorrect shown after each attempt. One sheet of notes and a calculator allowed; closed-book, closed-internet. Practice questions posted on Ed Discussions before each quiz opens.
- **Reports.** Four scored reports — Supervised Learning (SL), Optimization & Uncertainty in Learning (OL), Unsupervised Learning (UL), and Reinforcement Learning (RL) — covering programming and analysis. Reports must be written in LaTeX on Overleaf; code must use Private Georgia Tech GitHub repos (personal GitHub is prohibited and unscored). No rubric is provided (by pedagogical design), though an extensive internal rubric and a calibrated cross-staff grading system are used. Feedback explaining errors and successes is provided and is part of the learning goals.
- **Reviewer Response** *(change since Summer 2025, applies to Fall 2025).* A mechanism to edit and respond to feedback: within one week of a grade being posted, submit a two-page-maximum response with edits made and reviewer feedback. A proper Reviewer Response needs the initial submission, revised submission, and two-page response. If satisfactory, half the missed points are returned (e.g., 70/100 → 85/100). Applies only to the SL, OL, and UL reports (the RL report's feedback releases too close to term end).
- **Final Exam.** A digital, closed-book final exam administered via Canvas and Honorlock.
- **Final Letter Grade.** A curve is applied to the overall course grade at term end at the instructor's discretion (individual assignments are not curved). Historically most students earn grades in the A to B range, though exact cutoffs vary by term.

*Note:* a midterm administered in previous semesters has been removed. This term introduces a newly modified unit, an additional quiz from the summer, three updated quizzes, and the Reviewer Response, so assignment averages and overall grades are expected to shift slightly.

### Grade Component Weights

| Component | Weight |
|---|---|
| Reading/Writing Quiz | 5% |
| Hypothesis Quiz | 5% |
| Unit Quizzes (SL, OL, UL, RL — 5% each) | 20% |
| Reports (SL, OL, UL, RL — 12.5% each) | 50% |
| Final | 20% |

## Due Dates

All scored assignments are due at the indicated Eastern Time (ET); Canvas does not support Anywhere On Earth. Assignments are due at 11:59:00 PM ET on the date due, but since staff will not look at submissions until morning, the official late mark is 7:59:00 AM ET. Students should treat 11:59 PM as the internal deadline rather than the 7:59 AM official cutoff.

For **reports only**, late assignments incur a 20%-off-the-top per-day penalty for a maximum of 5 days, or a 0 grade. Exceptions require (1) a note from the appropriate authority and (2) immediate notification with a proper explanation. Approved late submissions are accepted only up to one full week after the due date; after that, a 0 is automatic. For cases needing longer than a week, dropping the course or requesting an incomplete is suggested.

For **quizzes**, since there are multiple attempts, each quiz is due at the exact due date. Preset due dates are maintained except for widespread outside forces preventing use of required technology; any change comes with at least 24-hour notice.

## Extra Credit

- A comprehensive problem set provided before the Final Exam (answers provided, not scored). Attempting and turning in all problems, with explanations, awards 1% to the overall course percentage.
- Significant contributions to the Ed Discussion board (at staff discretion) award 1% to the overall course percentage.
- Additional extra credit opportunities may be communicated on Ed Discussions.

## Office Hours and Other Channels

Non-recorded Office Hours run Monday through Thursday with TA team members (not required, but helpful). Friday Office Hours run weekly with a non-graded check-in quiz and a tangential lecture (often focused on SOTA methods/applications); the information disseminated in the Friday Office Hour should be considered required.

## Disclaimer

The instructor reserves the right to modify these plans as needed during the course; nothing will be done capriciously, changes won't be drastic, and students will be informed as far in advance as possible.

## Reading List

**Required Text:** Tom Mitchell, *Machine Learning*. McGraw-Hill, 1997. ([free online](http://www.cs.cmu.edu/afs/cs.cmu.edu/user/mitchell/ftp/mlbook.html))

**Optional Text:**

- Larry Wasserman, *All of Statistics*. Springer, 2010. ([online](http://www.stat.cmu.edu/~larry/all-of-statistics/)) — read Part 1 for an intro to Probability Theory.
- Richard Sutton and Andrew Barto, *Reinforcement Learning: An Introduction*. ([Nov 5, 2017 version](http://incompleteideas.net/book/bookdraft2017nov5.pdf))

**Prerequisites / Refreshers:** [Linear Algebra and Eigenproblems](https://github.com/pushkar/4641/raw/master/downloads/Eigenproblems.fm.pdf)

### Supervised Learning (SL1–SL8)

- **SL1: ML is the ROX** — Mitchell Ch 1
- **SL2: Decision Trees** — Mitchell Ch 3
- **SL3: Neural Networks** — Mitchell Ch 4
- **SL4: Instance-Based Learning** — Mitchell Ch 8
- **SL5: Ensemble Learning** — [Schapire's Introduction](https://github.com/pushkar/4641/raw/master/downloads/boosting.ps); [Jiri Matas and Jan Sochman's Slides](https://github.com/pushkar/4641/raw/master/downloads/adaboost_matas.pdf)
- **SL6: Kernel Methods and SVMs** — [An introduction to SVMs for data mining](https://www.cc.gatech.edu/classes/AY2008/cs7641_spring/handouts/yor12-introsvm.pdf); [Christopher Burges tutorial on SVMs for pattern recognition](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/svmtutorial.pdf); [Scholkopf's NIPS tutorial slides on SVMs and kernel methods](https://github.com/pushkar/4641/raw/master/downloads/svm-scholkopf.ps)
- **SL7: Computational Learning Theory** — Mitchell Ch 7
- **SL8: VC Dimensions** — *High-Dimensional Probability* by Vershynin (Chapter 8.3) (posted to Canvas)

### Optimization & Uncertainty in Learning (OL1–OL5)

- **OL1: Randomized Optimization** — Mitchell Ch 9
- **OL2: Deconstructing AdamW** — curated readings updated during the first couple weeks
- **OL3: Information Theory** — [No Free Lunch Theorem](https://ml-cs7641.s3.us-east-1.amazonaws.com/nfl-optimization-explanation.pdf); [Charles Isbell's Note on Information Theory](https://www.cc.gatech.edu/~isbell/tutorials/InfoTheory.fm.pdf); [An Introduction to Information Theory and Entropy](https://github.com/pushkar/4641/raw/master/downloads/gentle_intro_to_information_theory.pdf)
- **OL4: Bayesian Learning** — Mitchell Ch 6
- **OL5: Bayesian Inference** — Mitchell Ch 6

### Unsupervised Learning (UL1–UL4)

- **UL1: Clustering** — [Intuitive Explanation of EM](https://ml-cs7641.s3.us-east-1.amazonaws.com/em-intuitive-explanation.pdf); [Statistical View of EM](https://github.com/pushkar/4641/raw/master/downloads/em.pdf); [Jon Kleinberg's Impossibility Theorem for Clustering](https://www.cs.cornell.edu/home/kleinber/nips15.pdf)
- **UL2: Feature Selection** — Mitchell Ch 7
- **UL3: Feature Transformation** — [ICA: Algorithms and Applications](https://ml-cs7641.s3.us-east-1.amazonaws.com/ica-algorithms-and-applications.pdf); [Restructuring High Dimensional Data by Charles and Paul Viola](https://www.cc.gatech.edu/~isbell/papers/isbell-ica-nips-1999.pdf)
- **UL4: Manifold Learning** — Bishop Ch 12 (LLE & Isomap); *No Straight Lines Here* (blog by Aviral and LaGrow); *Visualizing Data with t-SNE* by van der Maaten and Hinton; Troy Whitfield Dimensionality Reduction (slides); Burges 2009 (extensive math, optional; posted to Canvas)

### Reinforcement Learning (RL1–RL5)

- **RL1: Markov Decision Processes** — Mitchell Ch 13
- **RL2: Reinforcement Learning** — Sutton and Barto, *Reinforcement Learning: An Introduction*, MIT Press, 1998 ([draft](http://incompleteideas.net/book/bookdraft2017nov5.pdf); chapters 2, 4, 6 helpful but not required); [Reinforcement Learning: A Survey](https://github.com/pushkar/4641/raw/master/downloads/kaelbling96reinforcement.pdf)
- **RL3: Game Theory** — [Andrew Moore's slides](http://www.cs.cmu.edu/~awm/tutorials.html)
- **RL4: Game Theory Continued** — curated readings updated during the first couple weeks
- **RL5: Horizon of Variants** — curated readings updated during the first couple weeks

## Software

- **Core ML (Python):** scikit-learn (the course workhorse for SL/UL — pipelines, CV, calibration, metrics); imbalanced-learn (resampling/class-weight tools); XGBoost / LightGBM / CatBoost (gradient-boosted trees for tabular baselines); scikit-learn-extra (extra algorithms such as k-medoids).
- **Deep Learning (for NNs):** PyTorch (+ Lightning for cleaner training loops; recommended for MLPs on tabular data); Keras / TensorFlow 2 (high-level API for quick prototypes); JAX / Flax (only for research-grade autodiff; not required). Do not use PyBrain (long unmaintained) — use PyTorch or Keras instead.
- **Optimization, Tuning, Experiment Tracking:** Optuna or Ray Tune (hyperparameter search with pruning); scikit-optimize (simple Bayesian optimization); MLflow or Weights & Biases (run/metric/parameter/artifact tracking).
- **Interpretability, Diagnostics, Calibration:** SHAP, LIME, ELI5; scikit-learn calibration or netcal; fairlearn.
- **Time Series (optional):** statsmodels, pmdarima, darts, prophet (not required for main assignments).
- **Reinforcement Learning & MDPs:** Gymnasium (maintained fork of Gym); Stable-Baselines3 (DQN, PPO, A2C, etc.); RLlib (scalable RL on Ray); MDPtoolbox (Python port); Murphy's MDP Toolbox (MATLAB).
- **Java / MATLAB Ecosystem:** WEKA; SMILE (Java/Scala); Deeplearning4j; ABAGAIL (Java, limited momentum); MATLAB Statistics & Machine Learning Toolbox, Dellaert's Clustering, MDP toolbox.
- **Data & Visualization:** pandas / polars; NumPy; matplotlib / plotly / altair.
- **Environments & Notebooks:** Anaconda/conda-forge or mamba/uv; JupyterLab / VS Code / Colab.

## Version Control

- 08/17/2025 — TJL published the course for the Fall semester.
- 08/17/2025 — TJL updated the reading list for the Fall semester.
- 08/15/2025 — TJL updated course policies for changes in the Fall semester.
