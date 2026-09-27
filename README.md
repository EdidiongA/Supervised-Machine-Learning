# Comparative Study of Supervised Learning Algorithms

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikit-learn&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-notebook-F37626?logo=jupyter&logoColor=white)
![Course](https://img.shields.io/badge/Georgia%20Tech-CS%207641%20Machine%20Learning-B3A369)

Five supervised learning algorithms, each swept across hyperparameters, benchmarked on two binary classification datasets from the UCI Machine Learning Repository, with the datasets first examined through correlation analysis, PCA and hypothesis testing.

Built for CS 7641 Machine Learning at Georgia Tech.

---

## Contents

- [Overview](#overview)
- [Datasets](#datasets)
- [Algorithms compared](#algorithms-compared)
- [Project description](#project-description)
- [Getting started](#getting-started)
- [Repository structure](#repository-structure)
- [Tooling](#tooling)
- [Author](#author)
- [License](#license)

---

## Overview

| | |
|---|---|
| **Task** | Binary classification on two tabular datasets |
| **Models** | Decision Tree, Neural Network, Gradient Boosting, Support Vector Machine, k-Nearest Neighbors |
| **Method** | Hyperparameter sweeps per model, with training and validation comparison, on both datasets |
| **Data analysis** | Correlation matrices, PCA dimensionality reduction, null and alternate hypothesis checks |
| **Format** | A single Jupyter notebook, organised by dataset |

## Datasets

| Dataset | Source | Instances | Features | Target |
|---|---|---|---|---|
| Rice (Cammeo and Osmancik) | [UCI 545](https://archive.ics.uci.edu/dataset/545/rice+cammeo+and+osmancik) | 3,810 | 7 | Rice species: Cammeo or Osmancik |
| Spambase | [UCI 94](https://archive.ics.uci.edu/dataset/94/spambase) | 4,601 | 57 | Email: spam or not spam |

Both are fetched directly through the `ucimlrepo` package; no manual download is needed.

## Algorithms compared

| Algorithm | Library | Hyperparameters explored |
|---|---|---|
| Decision Tree | scikit-learn | Depth, split criteria, pruning |
| Neural Network | Keras | Architecture, activation, training epochs |
| Gradient Boosting | scikit-learn | Estimators, learning rate, depth |
| Support Vector Machine | scikit-learn | Kernel, regularisation |
| k-Nearest Neighbors | scikit-learn | Number of neighbours, distance weighting |

## Project description

This project carries out complex and comprehensive supervised machine learning tasks and analyses by implementing several machine learning models/algorithms (Decision Tree, Neural Network, Gradient Boosting, Support Vector Machine and k-Nearest Neighbor models, each with different hyper-parameters) on two datasets. The first dataset is a Rice (Cammeo and Osmancik) dataset, a multivariate binary classification dataset, obtained from the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/545/rice+cammeo+and+osmancik), for two types of rice species grown in Turkey (Cammeo and Osmancik). The dataset has 3810 instances and contains seven (7) features in the feature set (X). the target variable (y) is whether the rice species is Cammeo or Osmancik.</br>
The second dataset is a Spambase dataset, a multivariate binary classification dataset, obtained from the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/94/spambase), which classifies emails as spam or non-spam. The dataset has integer and real data types. The dataset has 4601 instances with 57 features in the feature set (X). The target variable (y) is whether or not the email is spam.</br>
Correlation matrix analysis, PCA dimensionality reduction analysis and null/alternate hypotheses checks are also carried out on the datasets to examine them closely

## Getting started

### Requirements

Python 3.8 or later and Jupyter.

```bash
pip install numpy pandas matplotlib seaborn scikit-learn keras imbalanced-learn umap-learn ucimlrepo jupyter
```

### Run the notebook

```bash
jupyter notebook Supervised_Learning_for_GitHub.ipynb
```

The notebook is organised in two sections, one per dataset. Each section loads the data from UCI, examines it (correlation matrix, PCA, hypothesis checks), then trains and evaluates each of the five models across its hyperparameter sweep. Run the cells top to bottom.

## Repository structure

```
.
├── README.md
└── Supervised_Learning_for_GitHub.ipynb   # Full analysis, both datasets, all five models
```

## Tooling

| Purpose | Library |
|---|---|
| Data loading | ucimlrepo, pandas |
| Analysis and dimensionality reduction | NumPy, scikit-learn (PCA), UMAP |
| Class balancing | imbalanced-learn |
| Models | scikit-learn, Keras |
| Visualisation | Matplotlib, Seaborn |

## Author

**Edidiong-Abasi Anwanane**  
MSc Computer Science, Georgia Institute of Technology  
[Portfolio](https://edidionga.github.io) · [LinkedIn](https://www.linkedin.com/in/edidiong-abasi-anwanane/) · [GitHub](https://github.com/EdidiongA)

## License

MIT. See [LICENSE](LICENSE).
