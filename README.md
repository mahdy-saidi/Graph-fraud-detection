# Graph-based fraud detection with VGAE on IEEE-CIS Dataset

## Overview
This project implements a graph-based fraud detection approach using Variational Graph Autoencoders (VGAE) inspired by the article:

**Reference:**  
_"Graph-Based Bitcoin Fraud Detection Using Variational Graph Autoencoders and Supervised Learning"_ (DOI: [10.1016/j.procs.2025.03.105](https://doi.org/10.1016/j.procs.2025.03.105))  

While the original article applies VGAE to Bitcoin transactions, our goal is to adapt this approach to a simulated credit card transaction dataset, a Kaggle dataset that was generated using Sparkov Data Generation (Github tool created by Brandon Harris).

---

## Dataset

We are using the Credit Card Transactions Fraud Detection dataset from Kaggle: [Kaggle competition page](https://www.kaggle.com/datasets/kartik2112/fraud-detection/data)

**Files required:**
- `fraudTrain.csv`
- `fraudTest.csv`  

**Dataset folder structure (required for the repository):**


Ensure the CSV files are placed inside the `data/` folder at the repository root.

```bash
repository_root/
│
├─ data/
│  ├─ fraudTrain.csv
│  └─ fraudTest.csv
│
```

## Motivation
Traditional fraud detection models rely on tabular features. Graph-based methods provide the advantage of capturing relational patterns, such as connections between users, cards, devices, and transactions.