# 📚 COMPSCI 361 — Machine Learning Coursework & Projects

A collection of coursework, assignments, and group projects completed for **COMPSCI 361 — Machine Learning** at the **University of Auckland**.

🌐 **Live site:** [https://jeremiahpan23.github.io/ML-coursework-projects/](https://jeremiahpan23.github.io/ML-coursework-projects/)

---

## ✨ Overview

This repository hosts the reports and Jupyter notebooks for the assignments and group projects of COMPSCI 361. Each piece of work explores a different machine-learning problem — from data exploration and feature engineering to model training, evaluation, and critical analysis.

The companion website (linked above) provides a clean, browsable interface where every assignment can be opened directly as a rendered HTML report with a single click.

---

## 🎓 Course Information

| Field | Detail |
|-------|--------|
| **Course** | COMPSCI 361 — Machine Learning |
| **Institution** | University of Auckland |
| **Maintainer** | Jeremiah (Jiaxin) Pan |

---

## 📂 Assignments

> **⚠️ Flagship project:** Assignment 3 (BBC News Classification) is the most comprehensive deliverable this semester. It is featured as the hero project on the landing page and described in detail first, below.

| # | Title | Type | Report | Notebook |
|---|-------|------|:------:|:--------:|
| **A3** | **BBC News Classification** ⭐ FLAGSHIP | **Group Project · Group 4** | **[HTML](./A3_Group_4.html)** | **[ipynb](./A3_Group_4.ipynb)** |
| HW1 | Decision Tree Learning | Individual Homework | [HTML](./CS361_HW1_PAN.html) | [ipynb](./CS361_HW1_PAN.ipynb) |
| HW2 | Naive Bayes Text Classification | Individual Homework | [HTML](./CS361_HW2_Pan.html) | [ipynb](./CS361_HW2_Pan.ipynb) |

### Assignment 3 — BBC News Classification *(Flagship · Group Project)*

The largest, most rigorous piece of work produced this semester — a full end-to-end supervised text-classification pipeline on the BBC News dataset, delivered by a 5-person team. The project benchmarks **four different model families** (Naive Bayes, kNN, SVM with Linear and RBF kernels, and an ANN/MLP), conducts **5-fold cross-validation with GridSearchCV** on each, compares them on weighted F1, and analyses generalisation via a training-size study.

- **Dataset:** BBC News — 428 training articles, 106 testing articles (tech vs. entertainment)
- **Team:** Jeremiah (Jiaxin) Pan [Group Leader], Zhenyu Xiao, Fanling Zeng, Tingrui Li, Sicheng Li
- **Scope:** 5 people · 4 models · 4 major tasks · ≈ 13,500 extracted features

**Tasks covered:**

1. **Task 1 — Exploratory Data Analysis** — feature extraction with CountVectorizer / TF-IDF, top-50 term frequency plots, per-class frequency and class-balance visualisations.
2. **Task 2 — Classification Models Learning** — Naive Bayes (Multinomial) with likelihood-ratio & discriminative-word analysis, kNN (multiple distance metrics, k sensitivity, PCA decision boundaries), SVM (Linear soft-margin + RBF kernel with C/γ study, PCA boundaries), ANN/MLP (Truncated SVD dimensionality reduction, hidden-unit sweep).
3. **Task 3 — Classification Quality Evaluation** — 5-fold CV hyperparameter tuning for all four models, side-by-side weighted F1 comparison on the test set, plus a training-fraction impact study (test F1 vs. m).
4. **Task 4 — Insights Summary** — cross-model findings, EDA insights, and a final recommendation (**Linear SVM with C=1** is both the strongest and most reliable predictor, while Naive Bayes is the most interpretable).

**Techniques & tools:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, TF-IDF / CountVectorizer feature extraction, PCA & Truncated SVD projections, 5-fold CV with GridSearchCV, weighted F1, decision-boundary visualisation.

---

### Homework 1 — Decision Tree Learning *(Individual)*

A decision-tree classifier built entirely from scratch with NumPy. The implementation covers the full ID3-style learning procedure — entropy-based information gain, an exhaustive search-and-score routine to find the best split, recursive tree building, and configurable depth control. The model is evaluated on a wine-quality dataset binarised into good (quality ≥ 7) vs. not-good wines, followed by a critical reflection on splitting-criterion choices and overfitting.

- **Dataset:** Wine Quality — binarised (quality ≥ 7 vs. < 7)
- **Author:** Jeremiah (Jiaxin) Pan

**Tasks covered:**

1. **Coding** — (1-A) basic decision-tree learning procedure with information gain and best-split search; (1-A & 1-B) recursive tree building with depth control; (1-B) discussion of depth levels 2 / 3 / 4; (1-C) test procedure and evaluation.
2. **Reflection** — analysis of changing the splitting criterion and the effect of depth on generalisation.

**Techniques & tools:** `numpy`, decision trees from scratch, entropy, information gain, recursive splitting, depth control, binary classification.

### Homework 2 — Naive Bayes Text Classification *(Individual)*

A Multinomial Naive Bayes classifier implemented from scratch in NumPy, with probability computations performed in log-space to avoid floating-point underflow. Starting from a standard model on preprocessed abstract texts, the work explores model extensions (n-gram features), empirical hyperparameter tuning, and a rigorous evaluation against a null baseline.

- **Dataset:** Abstract texts — binary classification
- **Author:** Jeremiah (Jiaxin) Pan

**Tasks covered:**

1. **Data Representation, Preprocessing & Standard Implementation** — text cleaning and a from-scratch Naive Bayes classifier in log-space.
2. **Model Extensions & Modifications** — enhancements addressing Naive Bayes assumptions (e.g. n-gram features).
3. **Hyper-parameters Tuning** — empirical tuning of feature-extraction parameters (e.g. `ngram_range`).
4. **Evaluation Procedure** — 80/20 train/validation split with a null (majority-class) baseline.
5. **Results & Analysis** — accuracy comparison (Null ≈ 50.6%, Standard NB ≈ 92.8%).

**Techniques & tools:** `numpy`, Multinomial Naive Bayes from scratch, log-space probabilities, n-grams, train/validation split, null baseline, accuracy evaluation.

---

## 📁 Repository Structure

```
ML-coursework-projects/
├── index.html              # Landing page served by GitHub Pages
├── README.md               # This file
├── CS361_HW1_PAN.html      # Homework 1 — rendered HTML report
├── CS361_HW1_PAN.ipynb     # Homework 1 — Jupyter notebook source
├── CS361_HW2_Pan.html      # Homework 2 — rendered HTML report
├── CS361_HW2_Pan.ipynb     # Homework 2 — Jupyter notebook source
├── A3_Group_4.html         # Assignment 3 — rendered HTML report
└── A3_Group_4.ipynb        # Assignment 3 — Jupyter notebook source
```

---

## 🌍 Viewing the Work

There are three ways to view any assignment:

1. **Website (recommended):** Open the [live site](https://jeremiahpan23.github.io/ML-coursework-projects/) and click an assignment card to open its rendered HTML report.
2. **Directly on GitHub:** Click any `*.html` or `*.ipynb` file in this repository. Notebooks render preview directly on GitHub.
3. **Locally:** Clone the repo and open the `.html` files in a browser, or run `jupyter notebook` to open the `.ipynb` files.

```bash
git clone https://github.com/JeremiahPan23/ML-coursework-projects.git
```

---

## 🚀 Enabling the Website (GitHub Pages)

The site is served from the `main` branch via GitHub Pages. If it has not been enabled yet:

1. Go to **Settings → Pages** in the repository.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Select branch **`main`** and folder **`/ (root)`**, then click **Save**.
4. After a minute, the site will be live at the URL above.

---

## 📝 License

This repository contains academic coursework and is shared for educational and portfolio purposes. Please do not copy or submit this work as your own. All code and reports are the intellectual property of the authors listed above.
