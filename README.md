# Graph-based fraud detection with VGAE on IEEE-CIS Dataset

## Overview
This project implements a graph-based fraud detection approach using Variational Graph Autoencoders (VGAE) inspired by the article:

**Reference:**  
_"Graph-Based Bitcoin Fraud Detection Using Variational Graph Autoencoders and Supervised Learning"_ (DOI: [10.1016/j.procs.2025.03.105](https://doi.org/10.1016/j.procs.2025.03.105))  

While the original article applies VGAE to Bitcoin transactions, our goal is to adapt this approach to the IEEE-CIS Fraud Detection dataset, a Kaggle competition dataset containing anonymized credit card transaction data.

---

## Dataset

We are using the IEEE-CIS Fraud Detection dataset from Kaggle:  
[Kaggle competition page](https://www.kaggle.com/competitions/ieee-fraud-detection)

**Files required:**
- `train_transaction.csv` / `test_transaction.csv` – transactional features  
- `train_identity.csv` / `test_identity.csv` – identity/device features  

**Dataset folder structure (required for the repository):**


> Ensure the CSV files are placed inside the `data/` folder at the repository root.

```bash
repository_root/
│
├─ data/
│  ├─ train_transaction.csv
│  ├─ test_transaction.csv
│  ├─ train_identity.csv
│  └─ test_identity.csv
│
```

## Motivation
Traditional fraud detection models rely on tabular features. Graph-based methods provide the advantage of capturing relational patterns, such as connections between users, cards, devices, and transactions.