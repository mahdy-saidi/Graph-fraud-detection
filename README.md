# Graph-based fraud detection

## Overview
This project implements a graph-based fraud detection approaches.

---

## Dataset

We are using the Credit Card Transactions Fraud Detection dataset from Kaggle: [Kaggle dataset page](https://www.kaggle.com/datasets/kartik2112/fraud-detection/data)

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
Traditional fraud detection models rely on tabular features. Graph-based methods provide the advantage of capturing relational patterns, such as connections between users, cards, and transactions.