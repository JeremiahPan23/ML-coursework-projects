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

| # | Title | Type | Report | Notebook |
|---|-------|------|:------:|:--------:|
| A3 | BBC News Classification | Group Project · Group 4 | [HTML](./A3_Group_4.html) | [ipynb](./A3_Group_4.ipynb) |

### Assignment 3 — BBC News Classification *(Group Project)*

A complete supervised text-classification pipeline built on the BBC News dataset, classifying articles as either **tech** or **entertainment**. The project walks through the full machine-learning workflow: from exploratory data analysis and feature extraction, through training and tuning four different classifiers, to a rigorous comparative evaluation.

- **Dataset:** BBC News — 428 training articles and 106 testing articles (binary: tech vs. entertainment)
- **Group 4 members:** Jeremiah (Jiaxin) Pan *(Group Leader)*, Zhenyu Xiao, Fanling Zeng, Tingrui Li, Sicheng Li

**Tasks covered:**

1. **Exploratory Data Analysis** — feature extraction with `CountVectorizer` / TF-IDF, term-frequency and class-distribution visualizations.
2. **Classification Models Learning** — Multinomial Naive Bayes, k-Nearest Neighbours, Support Vector Machines (Linear & RBF kernels), and an Artificial Neural Network (MLP with Truncated SVD).
3. **Classification Quality Evaluation** — 5-fold cross-validation hyperparameter tuning (`GridSearchCV`), model comparison using weighted F1 score, and analysis of training-data-size impact.
4. **Insights Summary** — discussion of findings across models and the overall learning outcomes.

**Techniques & tools:** `scikit-learn`, TF-IDF / CountVectorizer, PCA, Multinomial Naive Bayes, kNN, Linear & RBF SVM, MLP/ANN, 5-fold cross-validation, GridSearchCV, weighted F1 evaluation, matplotlib/seaborn visualizations.

---

## 📁 Repository Structure

```
ML-coursework-projects/
├── index.html              # Landing page served by GitHub Pages
├── README.md               # This file
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
