# ECON 524: Big Data Econometrics — Lab

This repository contains the **lab (discussion section) materials** for **ECON 524: Big Data Econometrics**. The lab complements the Monday/Wednesday lectures with hands-on Python implementation of machine learning methods for prediction and causal inference, using simulated and real economic data.

### Lab logistics (Fall 2026)

- **Meets:** Friday 10:00–10:50 AM, Rich 108 (the same room as lecture, meeting after the week's MW lectures)
- **First lab:** Friday, August 28, 2026 *(confirm against the official Fall 2026 calendar)*
- **Weight:** The lab is **25% of the course grade**, alongside the midterm (35%, Oct 21) and final exam (40%, Dec 14). See **Lab Grading** below for the breakdown.
- **Instructor:** Zheng Fang (zheng.fang@emory.edu)
- **Lab Instructor:** Joel Reyes Mora (joel.reyes.mora@emory.edu)
- **Grader:** Marcelo Ortiz-Villavicencio (marcelo.ortiz@emory.edu)

## Course Overview

ECON 524 studies how machine learning methods can support credible empirical research in economics. The course moves from linear and nonlinear prediction methods to the identification of causal effects, and finally to **debiased machine learning (DML)** — a framework for valid statistical inference when nuisance parameters are high-dimensional. The lab exists to turn the lecture's theory into working Python code:

- **Linear ML methods** — LASSO, cross-validation, and regularized logistic regression for classification
- **Nonlinear ML methods** — decision trees, random forests, boosting, and the basics of deep learning
- **Causal inference fundamentals** — the potential outcomes framework, unconfoundedness, instrumental variables/LATE, and difference-in-differences
- **Debiased machine learning** — model-based DML and DML via the Riesz representer, for inference with high-dimensional nuisances

## Policy and Guidance on the Use of Generative AI

Unless a specific assignment says otherwise, you may use generative AI tools while working on lab assignments. Doing so carries no penalty **as long as you acknowledge it**, using the statement format below. Failing to acknowledge AI use is a violation of the Honor Code, treated the same as failing to cite any other source.

**What AI can help with:** planning an approach, clarifying a concept, writing or debugging code, and checking your work. It should support your own reasoning, not replace it — the assignments exist to build skills you're expected to have yourself.

**Before you rely on an AI response, it helps to think through four things:**
1. *Context* — what's the goal, and what inputs or sources does the tool actually need to do this well?
2. *Task* — what exactly should it produce, and under what constraints?
3. *Follow-up* — what assumptions or possible errors should you push back on or ask it to double check?
4. *Checking* — how will you verify the result yourself, independent of the tool?

**You are responsible for everything you submit**, regardless of how it was produced. You should understand your work well enough to explain it and, if asked, reproduce its core reasoning or code without AI assistance. Fluent, well-formatted output is not the same as correct output: AI tools can generate plausible-looking but wrong derivations, fabricated citations, or code that runs without actually answering the question. Verify anything substantive independently — against course material, original sources, hand-checkable cases, or your own tests — and never cite an AI response itself as the source of a factual claim.

**Required acknowledgment.** Every lab assignment submission must end with one of the following:

> **AI-use statement:** No generative AI was used.

or

> **AI-use statement:** I used [tool(s)] for [purpose / which part of the assignment]. Its contribution was [what it generated, revised, or checked]. I verified or revised the output by [how].

A full transcript isn't required unless an assignment says so. This statement is in addition to, not a substitute for, normal citation of any other sources you use.

## Lab Grading

The lab is **25% of the course grade**, scored out of **25 points** (1 lab point = 1% of the course grade). The scheme rewards consistent attendance and hands-on practice rather than exam-style performance.

| Component | Points | How it works |
|---|---|---|
| Attendance & in-lab work | 11 | 13 sessions, 1 point each, **capped at 11** |
| Biweekly assignments | 14 | 7 assignments × 2 points each |
| **Total** | **25** | |

### Attendance & in-lab work — 11 points

- There are 13 lab sessions. Each session is worth 1 point, and the total is **capped at 11**, so you may miss up to two sessions with no penalty.
- Attending fewer than 11 sessions costs 1 point for each session below 11. **Attendance at 11 sessions is the minimum expectation for the lab.**
- **Excused absences** (documented illness, family emergency, religious observance, university-sanctioned travel) do not count against the 11.

### Biweekly assignments — 14 points

- **7 assignments**, released roughly every two weeks, **2 points each**. All 7 count toward the grade.
- Each assignment applies the method from the preceding one or two labs: a short implementation or replication exercise with a few sentences of interpretation. They are meant to be completed in a few hours, not to be term papers.
- Each assignment is graded on a simple rubric — **code reproduces / runs (40%), correct estimates and answers (40%), interpretation (20%)**.
- Collaboration on approach is allowed; every student submits their own code and write-up.
- **No late work is accepted.** A missed assignment receives 0. Because the assignments are low-stakes (2 points each) and frequent, a single missed assignment has a limited effect on the overall grade; the flexibility for illness or travel is built into the attendance cap.

## Repository Structure

```
├── labs/          # Notebooks / scripts for each lab session
├── slides/        # Lab slides and handouts
├── data/          # Datasets used in lab exercises
├── assignments/   # Problem sets tied to the lab methods
└── utils/         # Helper functions and shared utilities
```

This layout grows over the term; not every directory is populated at the start of the semester.

## Getting Started

### Prerequisites

- Econ 520, 526, and 725 (or permission of the 4+1 Director), per the course syllabus
- Comfort with a scripting language for data analysis

### Language

Lab exercises are provided in **Python**, matching the lecture notebooks and slides.

### Installation (Python)

1. Clone this repository:
```bash
git clone https://github.com/[username]/econ524-big-data-econometrics-lab.git
cd econ524-big-data-econometrics-lab
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Lab:
```bash
jupyter lab
```

## Key Topics Covered

### 1. Linear Machine Learning Methods
- Big data vs. traditional data; the bias–variance trade-off
- LASSO regression, penalty selection, and cross-validation
- Logistic regression and regularized classification

### 2. Nonlinear Machine Learning Methods
- Decision trees, random forests, and boosting
- Basics of deep learning (neural networks)

### 3. Fundamentals of Causal Inference
- The potential outcomes framework and unconfoundedness
- Instrumental variables and local average treatment effects (LATE)
- Difference-in-differences

### 4. Debiased Machine Learning
- Motivations: why plug-in ML estimates of causal parameters can be biased
- Model-based debiased machine learning
- Debiased machine learning via the Riesz representer

## Resources

### Textbooks
- James, G., Witten, D., Hastie, T., Tibshirani, R., & Taylor, J. (2023). *An Introduction to Statistical Learning: With Applications in Python*. Springer. ([statlearning.com](https://www.statlearning.com))
- Chernozhukov, V., Hansen, C., Kallus, N., Spindler, M., & Syrgkanis, V. (2024). *Applied Causal Inference Powered by ML and AI*. Online manuscript. ([causalml-book.org](https://causalml-book.org))

### Selected additional readings (see syllabus for full list)
- Imbens, G. W. (2004). Nonparametric estimation of average treatment effects under exogeneity: A review. *Review of Economics and Statistics*.
- Imbens, G. W., & Angrist, J. D. (1994). Identification and estimation of local average treatment effects. *Econometrica*.
- Baker, A., Callaway, B., Cunningham, S., Goodman-Bacon, A., & Sant'Anna, P. H. C. (2026). Difference-in-differences designs: A practitioner's guide. *Journal of Economic Literature*.
- Farrell, M. H., Liang, T., & Misra, S. (2021). Deep neural networks for estimation and inference. *Econometrica*.
- Chernozhukov, V., Newey, W. K., Quintas-Martinez, V., & Syrgkanis, V. (2024). Automatic debiased machine learning via Riesz regression. *arXiv:2104.14737*.
- Ahrens, A., Chernozhukov, V., Hansen, C., Kozbur, D., Schaffer, M., & Wiemann, T. (2026). An introduction to double/debiased machine learning. *arXiv:2504.08324*.

### Software
- **Python**: `numpy`, `pandas`, `scikit-learn`, `statsmodels`, plus a deep learning library (e.g. `torch` or `tensorflow`) and a DML library (e.g. `doubleml` or `econml`)

## Course Policies (from the course syllabus)

- **Regrading requests** must be made within one week of receiving an exam, directed first to the grader.
- **Attendance extra credit:** attendance at lecture is not mandatory but not tracked for the lab grade above; missing no more than three *lectures* earns 5% course extra credit (separate from lab attendance).
- **Academic integrity:** the Honor Code applies to all lab assignments and exams. See the course syllabus for full policy language.
- **Accessibility:** students needing accommodations should register with Emory's Department of Accessibility Services (DAS) as early as possible in the semester.

## Contributing

If you find errors or have suggestions for improvements:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

## License

These materials are provided for educational use as part of ECON 524. Please cite appropriately when reusing these materials in your own work.

## Contact

For questions about the lab materials:
- Open an issue in this repository
- Contact the lab instructor during office hours
- Post on the course discussion forum

---

*This repository is for educational purposes as part of ECON 524, Fall 2026, Emory University.*
