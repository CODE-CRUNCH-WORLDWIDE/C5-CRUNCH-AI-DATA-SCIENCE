# C5 · Crunch AI / Data Science

> A free, open-source **12-week data-science + classical-ML track** for engineers who already know Python. NumPy through PyTorch, with the experimentation discipline employers actually want. C1 graduate → mid-level ML / data scientist.

[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](LICENSE)
[![Python 3.11+](https://img.shields.io/badge/python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Built in the open](https://img.shields.io/badge/built-in%20the%20open-7C3AED.svg)](https://github.com/CODE-CRUNCH-CLUB)

C5 takes you from "I know Python" to "I can take a real dataset, do honest analysis, build a model, evaluate it without fooling myself, and ship it behind an API." It is not a survey course — every week ends with a deliverable that pushes to a portfolio repo.

---

## Standards & equivalency

> C5 stands in for a university's machine-learning course, and for the learning half of its data-mining and artificial-intelligence courses.

**University equivalent.** Three of them, not one. **Machine Learning** — `CAP 4611`, `CS 4780`, `CS 229`. **Data Mining** — `CAP 4770`, `CS 4780`, `CS 412`. **Artificial Intelligence** — `CAP 4630`, `CS 4300`, `CS 188`.

Coverage: **full** against Machine Learning, **partial** against Data Mining and against Artificial Intelligence. Partial has a precise meaning in each case, and in neither case does it mean "most of it".

Against **Data Mining**, partial means one named method is missing. C5 teaches the preparation half — reading, cleaning and integrating real tabular data — and the modelling and evaluation half — clustering, mixture models, dimensionality reduction, supervised prediction, model selection and leakage-free experiment design. It does not teach classical association-rule mining: Apriori, FP-growth, support and confidence, the market-basket formulation. That is the single row marked `lighter` against Data Mining below, and it is declared again at the end of this section.

Against **Artificial Intelligence**, partial is a matter of which half. An AI section is roughly two courses bolted together: the symbolic half (state-space search, constraint satisfaction, logical knowledge representation and the planning built on them) and the learning half. C5 is the learning half, taught deeper than an AI section reaches — complete pipelines, model choice, training, evaluation and explanation, with three weeks of architecture work past where an AI section stops. It is not the symbolic half at all, and does not pretend to be. Those are the two rows marked `lighter` against Artificial Intelligence below.

C5 carries no credit, no transcript entry, no accreditation and no proctored exam. The equivalence is one of **content and skill**: the outcomes below are taught here at the same depth or deeper except where a row says otherwise, and every one of them is assessed. What a registrar records is not something an open repository can give you.

| University outcome | Where this course teaches it | Depth |
| --- | --- | --- |
| **Machine Learning** — the supervised workflow: framing, splitting, fitting, evaluating, and the discipline that keeps the test set honest | [Week 04](curriculum/week-04-ml-workflow-and-linear-models/) | deeper |
| **Machine Learning** — linear and logistic regression: the loss, the closed-form and gradient-descent solutions, and the assumptions behind the fit | [Week 04](curriculum/week-04-ml-workflow-and-linear-models/) | deeper |
| **Machine Learning** — regularization: ridge, lasso and elastic net, with the penalty chosen by cross-validation rather than by feel | [Week 04](curriculum/week-04-ml-workflow-and-linear-models/) | same |
| **Machine Learning** — the bias-variance decomposition, learning curves, and reading a model's failure as one or the other | [Week 04](curriculum/week-04-ml-workflow-and-linear-models/) | same |
| **Machine Learning** — decision trees, and the impurity criteria that drive the recursive split | [Week 05](curriculum/week-05-trees-forests-boosting/) | deeper |
| **Machine Learning** — ensembles: bagging, random forests, and gradient boosting as functional gradient descent | [Week 05](curriculum/week-05-trees-forests-boosting/) | deeper |
| **Machine Learning** — unsupervised learning: k-means, hierarchical and density-based clustering, and Gaussian mixtures fitted by EM | [Week 06](curriculum/week-06-clustering-and-dimensionality-reduction/) | same |
| **Machine Learning** — dimensionality reduction: PCA from the covariance eigendecomposition, and nonlinear embeddings for visualization | [Week 06](curriculum/week-06-clustering-and-dimensionality-reduction/) | same |
| **Machine Learning** — neural networks: the forward pass, backpropagation derived from the chain rule, and stochastic gradient descent | [Week 07](curriculum/week-07-neural-networks-from-scratch/) | deeper |
| **Machine Learning** — training a network with a modern framework: autograd, optimizers, batching, devices and checkpoints | [Week 08](curriculum/week-08-pytorch-fundamentals/) | deeper |
| **Machine Learning** — classification and regression metrics, and choosing the one that fits an imbalanced problem | [Week 04](curriculum/week-04-ml-workflow-and-linear-models/) | deeper |
| **Machine Learning** — interpreting a fitted model: split-gain importance, permutation importance and SHAP, each with its failure mode | [Week 05](curriculum/week-05-trees-forests-boosting/) | deeper |
| **Machine Learning** — carry a complete project end to end and defend the result in writing | [Week 12](curriculum/week-12-capstone-end-to-end-ml-with-deploy/) | deeper |
| **Data Mining** — prepare real data for analysis: mixed types, missing values, encoding errors, time zones, and joining sources that disagree | [Week 02](curriculum/week-02-pandas-honestly/) | deeper |
| **Data Mining** — exploratory analysis and visualization of a dataset before any model is fitted | [Week 03](curriculum/week-03-visualization-that-doesnt-lie/) | deeper |
| **Data Mining** — cluster analysis: partitioning, hierarchical and density-based methods, and defending the number of clusters | [Week 06](curriculum/week-06-clustering-and-dimensionality-reduction/) | same |
| **Data Mining** — dimensionality reduction and the projection of high-dimensional records into a readable space | [Week 06](curriculum/week-06-clustering-and-dimensionality-reduction/) | same |
| **Data Mining** — classification and prediction from mined data, with tree-based methods as the tabular default | [Week 05](curriculum/week-05-trees-forests-boosting/) | same |
| **Data Mining** — evaluate a mined model honestly: held-out data, cross-validation, and the leaks that inflate a score | [Week 04](curriculum/week-04-ml-workflow-and-linear-models/) | deeper |
| **Data Mining** — association-rule mining: support, confidence, lift, and the Apriori and FP-growth algorithms over transaction data | not taught; the nearest unsupervised structure-finding this course does is the clustering and mixture work in [Week 06](curriculum/week-06-clustering-and-dimensionality-reduction/) | lighter |
| **Artificial Intelligence** — machine learning as the AI subfield: learn a function from labelled data and measure what was learned | [Week 04](curriculum/week-04-ml-workflow-and-linear-models/) | deeper |
| **Artificial Intelligence** — neural networks and the learned representation, from a single neuron to a trained deep model | [Week 07](curriculum/week-07-neural-networks-from-scratch/) | deeper |
| **Artificial Intelligence** — perception: convolutional architectures over images, and reusing a representation somebody else trained | [Week 09](curriculum/week-09-cnns-and-transfer-learning/) | deeper |
| **Artificial Intelligence** — learning without labels, and reasoning about structure the data was not annotated with | [Week 06](curriculum/week-06-clustering-and-dimensionality-reduction/) | same |
| **Artificial Intelligence** — experimental method: baselines, held-out evaluation, and reporting a result you would defend | [Week 12](curriculum/week-12-capstone-end-to-end-ml-with-deploy/) | deeper |
| **Artificial Intelligence** — classical search over a state space: uninformed and heuristic search, A\*, and adversarial search with minimax | not taught; the only search this course runs is the greedy best-split search inside the decision tree built in [Week 05](curriculum/week-05-trees-forests-boosting/) | lighter |
| **Artificial Intelligence** — constraint satisfaction, logical knowledge representation, and the planning built on them | not taught; [Week 12](curriculum/week-12-capstone-end-to-end-ml-with-deploy/) frames a problem as a target, a window, a metric and a baseline, where an AI section would frame it as variables, constraints and a goal test | lighter |

Every row not marked `lighter` points at a week that **assigns work** on that outcome — a graded exercise, a challenge, homework, a quiz item, a mini-project or the capstone — not merely a week that mentions it.

**The industry bar.** What an employer expects of somebody paid to do data-science and machine-learning work, and where this course makes the learner do it. Where the course does not yet clear a clause, the row says so rather than dressing up the nearest thing.

| What the job expects | Where this course does it |
| --- | --- |
| Work lands as a commit in a repository you own, not a notebook on your desktop | every mini-project and every Week 10–11 challenge is specified as a push to `crunch-ai-portfolio-<yourhandle>`, e.g. [`curriculum/week-10-sequence-models-rnn-lstm-gru/challenges/challenge-02-lstm-vs-gru-bake-off.md`](curriculum/week-10-sequence-models-rnn-lstm-gru/challenges/challenge-02-lstm-vs-gru-bake-off.md) |
| You read an implementation you did not write and form a judgement on it | [`curriculum/week-08-pytorch-fundamentals/exercises/SOLUTIONS.md`](curriculum/week-08-pytorch-fundamentals/exercises/SOLUTIONS.md) hands over a full reference implementation with the reasoning behind each choice, and [`curriculum/week-03-visualization-that-doesnt-lie/challenges/challenge-01-recreate-an-FT-chart.md`](curriculum/week-03-visualization-that-doesnt-lie/challenges/challenge-01-recreate-an-FT-chart.md) puts somebody else's published work in front of the learner and asks for a written critique. Neither is a defect-hunt through a working-but-wrong module; that review exercise is the one industry clause C5 does not yet clear in the form §0a describes |
| Tests exist, and the command to run them is written down | [`curriculum/week-01-numpy-from-scratch/exercises/README.md`](curriculum/week-01-numpy-from-scratch/exercises/README.md) names the `pytest` invocation per exercise file; the Week 8–11 solution files are written against a named headline test, and [`curriculum/week-09-cnns-and-transfer-learning/mini-project/rubric.md`](curriculum/week-09-cnns-and-transfer-learning/mini-project/rubric.md) scores a fresh-clone run and a `python -m py_compile` pass |
| You read the real error instead of guessing | [`curriculum/week-08-pytorch-fundamentals/lecture-notes/03-datasets-dataloaders-devices-and-checkpoints.md`](curriculum/week-08-pytorch-fundamentals/lecture-notes/03-datasets-dataloaders-devices-and-checkpoints.md) carries a symptom-to-cause table of the actual PyTorch runtime errors, and [`curriculum/week-02-pandas-honestly/lecture-notes/01-series-and-dataframes-mental-model.md`](curriculum/week-02-pandas-honestly/lecture-notes/01-series-and-dataframes-mental-model.md) reproduces the `SettingWithCopyWarning` text and traces what it is actually warning about |
| An experiment is reproducible by somebody else | seeds are a rubric line, not a suggestion — `random_state=42` in [`curriculum/week-05-trees-forests-boosting/challenges/challenge-01-feature-importance-vs-shap.md`](curriculum/week-05-trees-forests-boosting/challenges/challenge-01-feature-importance-vs-shap.md), `torch.manual_seed(42)` scored in [`curriculum/week-09-cnns-and-transfer-learning/mini-project/rubric.md`](curriculum/week-09-cnns-and-transfer-learning/mini-project/rubric.md), and a pinned `requirements.txt` plus a versioned data and model artifact required by [`curriculum/week-12-capstone-end-to-end-ml-with-deploy/README.md`](curriculum/week-12-capstone-end-to-end-ml-with-deploy/README.md) |
| Dependencies are isolated and pinned per project | [`curriculum/week-12-capstone-end-to-end-ml-with-deploy/lecture-notes/03-packaging-deploying-and-monitoring.md`](curriculum/week-12-capstone-end-to-end-ml-with-deploy/lecture-notes/03-packaging-deploying-and-monitoring.md), where the inference layer may depend on nothing outside `requirements.txt` and the one model file |
| A model is evaluated for who it fails, not only for its headline number | [`curriculum/week-12-capstone-end-to-end-ml-with-deploy/lecture-notes/02-evaluation-fairness-and-model-cards.md`](curriculum/week-12-capstone-end-to-end-ml-with-deploy/lecture-notes/02-evaluation-fairness-and-model-cards.md) — the slice-based audit, with a stated threshold and a written justification for it |
| The thing you built runs somewhere other than your laptop | [`curriculum/week-12-capstone-end-to-end-ml-with-deploy/lecture-notes/03-packaging-deploying-and-monitoring.md`](curriculum/week-12-capstone-end-to-end-ml-with-deploy/lecture-notes/03-packaging-deploying-and-monitoring.md) — a `predict.py`, a `serve.py`, and a publicly reachable URL the capstone rubric requires |
| The output is portfolio-grade: a stranger can clone it and know what you can do | [`curriculum/week-09-cnns-and-transfer-learning/mini-project/rubric.md`](curriculum/week-09-cnns-and-transfer-learning/mini-project/rubric.md) scores the clean-clone run directly, and the capstone adds a graded `HANDOFF.md` at [`curriculum/week-12-capstone-end-to-end-ml-with-deploy/README.md`](curriculum/week-12-capstone-end-to-end-ml-with-deploy/README.md) |
| A formatter, a linter, and a pipeline that runs on every push | not yet. C5 pins versions, sets seeds, and scores a `py_compile` pass, but it does not put the learner's work through a configured formatter, linter, or CI run. This is the second industry clause C5 does not clear, and it is declared with the gaps below |

**Beyond both bars.** Clearing the two floors is entry, not success. Open any of these and check it in under a minute.

| What we add | Which bar it beats | Where it lives |
| --- | --- | --- |
| Worked answers are published with the exercise, in full, with the reasoning behind every choice and the failure each guard prevents — not held back behind a deadline | both | [`curriculum/week-08-pytorch-fundamentals/exercises/SOLUTIONS.md`](curriculum/week-08-pytorch-fundamentals/exercises/SOLUTIONS.md) |
| Every quiz publishes its answer key in the same file, folded under the questions, with the reasoning rather than the letter | university | [`curriculum/week-01-numpy-from-scratch/quiz.md`](curriculum/week-01-numpy-from-scratch/quiz.md) |
| The learner implements what the framework hides — a reverse-mode autograd engine over a computation graph, before ever calling `loss.backward()` | university | [`curriculum/week-07-neural-networks-from-scratch/challenges/challenge-02-write-your-own-autograd.md`](curriculum/week-07-neural-networks-from-scratch/challenges/challenge-02-write-your-own-autograd.md) |
| Three weeks sit entirely past the outcome set of all three university courses — recurrence, attention, and a decoder-only transformer the learner reads line by line and trains against their own Week 10 baseline | university | [`curriculum/week-11-attention-transformers-and-mini-gpt/lecture-notes/03-decoder-only-and-mini-gpt.md`](curriculum/week-11-attention-transformers-and-mini-gpt/lecture-notes/03-decoder-only-and-mini-gpt.md) |
| A published result reproduced on the learner's own machine — the gradient-norm-by-timestep curve from Pascanu, Mikolov and Bengio 2013, measured rather than quoted | both | [`curriculum/week-10-sequence-models-rnn-lstm-gru/challenges/challenge-01-gradient-norms-by-depth.md`](curriculum/week-10-sequence-models-rnn-lstm-gru/challenges/challenge-01-gradient-norms-by-depth.md) |
| Model cards, dataset cards and a slice-based fairness audit are graded artifacts carrying a quarter of the capstone score — a thorough card outranks a better accuracy number | both | [`curriculum/week-12-capstone-end-to-end-ml-with-deploy/lecture-notes/02-evaluation-fairness-and-model-cards.md`](curriculum/week-12-capstone-end-to-end-ml-with-deploy/lecture-notes/02-evaluation-fairness-and-model-cards.md) |
| Every mini-project ships with the grader's rubric published in advance, point by point, so the learner can self-mark before submitting | both | [`curriculum/week-09-cnns-and-transfer-learning/mini-project/rubric.md`](curriculum/week-09-cnns-and-transfer-learning/mini-project/rubric.md) |
| A whole lecture on when the method is the wrong answer — the clustering that is an artifact of preprocessing, the elbow plot with no elbow, the segmentation that was a classification problem all along | university | [`curriculum/week-06-clustering-and-dimensionality-reduction/lecture-notes/03-when-clustering-is-not-the-answer.md`](curriculum/week-06-clustering-and-dimensionality-reduction/lecture-notes/03-when-clustering-is-not-the-answer.md) |

**Gaps we declare.** Three against the university bar, and they are the three the ledger records: C5 does not teach classical association-rule mining — support, confidence, lift, Apriori and FP-growth over transaction data; it does not teach classical state-space search, including A\* and minimax; and it does not teach constraint satisfaction or logical knowledge representation, or the planning built on them. Two against the industry bar: no unit yet puts a working-but-wrong implementation in front of the learner and asks for a ranked defect review, and no unit yet runs the learner's work through a configured formatter, linter or CI pipeline. Both are unbuilt work, not a claim we are withdrawing.

---

## Pathway summary

- **Full-time:** 12 weeks · ~36 hrs/week · ~432 hours
- **Working-engineer pace:** 6 months · ~18 hrs/week
- **Evening pace:** 12 months · ~9 hrs/week

See [`SYLLABUS.md`](SYLLABUS.md) for the full week-by-week breakdown across four phases.

---

## What you will be able to do at the end of 12 weeks

- **Read and clean** any reasonable real-world dataset in pandas — including all the edge cases (mixed types, missing values, encoding errors, time zones).
- **Build a complete ML pipeline** with scikit-learn from raw data to a trained model: split, vectorize, fit, evaluate, cross-validate, save.
- **Choose the right model** for a tabular problem: when linear regression suffices, when you need trees, when neural nets pay off, when classical statistics is more honest.
- **Train a small neural network** in PyTorch end-to-end: dataset, dataloader, `nn.Module`, optimizer, training loop, checkpointing, inference.
- **Explain a model's predictions** with SHAP or permutation importance — and know what those numbers do and don't mean.
- **Set up an experiment**: hold-out set, cross-validation, leakage-free preprocessing, fair baselines, statistical significance.
- **Ship a model behind an API** (FastAPI) and call it from a small frontend.
- **Read papers** at the level of mainstream ML conferences without getting lost.

---

## Who this is for

- **C1 graduate** who wants the data-science specialization.
- **Self-taught engineer** comfortable with Python and itching for data work.
- **CS / stats / engineering learner** preparing for an ML-adjacent first job.
- **Working engineer** transitioning into a data team.

Not for: pure beginners (do [C1](../C1-Code-Crunch-Convos/) first), researchers wanting publication-grade depth (this is engineering-grade, not academic), or people who specifically want LLMs/agents (those are in the upcoming Crunch Labs **C23 · Crunch Agents** track).

---

## Prerequisites

- **C1 Weeks 1–14** completed, or equivalent.
- Comfortable with: functions, classes, decorators, generators, list/dict comprehensions, exception handling, `pip` / `venv`.
- Some exposure to algebra and calculus — derivatives, vectors, basic matrix math. We re-teach the bits we need, but a complete blank slate makes Week 7 (NN from scratch) tough.
- A computer with ≥8 GB RAM. A GPU is nice for Week 8+ but not required — Google Colab's free tier handles every Week.

---

## What you ship

By the end of the program, your `crunch-ai-portfolio-<yourhandle>` GitHub repo contains:

1. **A vectorized image-processing notebook** (Week 1) — pure NumPy, no PIL.
2. **An EDA report** on a real public dataset (Week 2).
3. **A re-creation + critique** of three published charts (Week 3).
4. **A house-price prediction** project with both linear and tree-based models (Weeks 4–5).
5. **A clustering analysis** with justified k and 2D visualization (Week 6).
6. **A 2-layer NN trained from scratch in pure NumPy** on MNIST ≥ 95% accuracy (Week 7).
7. **A PyTorch version** of the same, with data augmentation, beating the NumPy version (Week 8).
8. **A fine-tuned pre-trained CNN** on a real image task (Week 9).
9. **An A/B test plan** for a real product question (Week 10).
10. **A FastAPI-served model** with experiment tracking and Docker (Week 11).
11. **A capstone project** end-to-end with a fairness/limitations section (Week 12).

That repo is the artifact you hand recruiters.

---

## Tools we use

| Tool | Role |
|------|------|
| **Python 3.11+** | Language |
| **NumPy** | The N-dimensional array; vectorization |
| **pandas** | DataFrames, IO, cleaning |
| **matplotlib · seaborn · plotly** | Visualization |
| **scikit-learn** | Classical ML |
| **PyTorch** | Deep learning |
| **Jupyter / VS Code notebooks** | Exploration |
| **FastAPI** | Model serving |
| **mlflow** | Experiment tracking |
| **Docker** | Packaging |
| **DuckDB / Polars** | Mentioned as faster pandas alternatives in stretch readings |

Everything is **free** and **open-source**. No paid Kaggle Pro, no proprietary AutoML SaaS, no required GPU rental — Google Colab's free tier handles the deep-learning weeks.

---

## Migration from legacy units

The existing `Unit-0` through `Unit-9` Jupyter notebooks remain available for now. Each is being rolled forward into the standardized weekly module layout used by C1, C16, C17, and C2. See the [SYLLABUS.md migration table](SYLLABUS.md#migration-from-the-legacy-units) for the mapping.

Contributors: each new week's PR should follow the [Code Crunch contribution guide](../CONTRIBUTING.md) and match the depth of [C1 Week 1](../C1-Code-Crunch-Convos/curriculum/week-01-python-foundations/).

---

## Next track after C5

- **[C17 · Crunch Pro Python Advanced](../C17-CRUNCH-PRO-PYTHON-ADVANCED/)** — for the runtime depth (async, performance, PyTorch internals).
- **[C15 · Crunch DevOps](../C15-CRUNCH-DEVOPS/)** — deploy your models in production.
- **C23 · Crunch Agents** (Tier 2 Labs) — for LLM / agentic systems beyond classical ML.

---

## License

GPL-3.0. See [LICENSE](LICENSE).

---

*C5 is part of the Code Crunch open-source curriculum.* [Master catalog ↗](../MASTER-CURRICULUM.md) · [Brand family ↗](../../assets/brand/BRAND-FAMILY.md)
