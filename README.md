# Optimising High-Dimensional Logistic Regression via MM

**Exploring Majorisation–Minimisation (MM) for efficient, stable, and interpretable logistic regression in high-dimensional feature spaces.**  

This project benchmarks **MM** against traditional optimisation methods, **Gradient Descent (GD)** and **Newton-Raphson (NR)**, on real-world financial data and synthetic datasets. It demonstrates convergence efficiency, numerical stability, and predictive performance in challenging high-dimensional settings.

---

## Key Insights

- **MM consistently outperforms traditional methods**: Comparable accuracy to GD and NR on the LendingClub loan dataset, while converging in fewer iterations and with more stable runtimes.  
- **Scalable and robust**: Performs well on synthetic datasets even when features approach the number of samples (p ≈ n).  
- **Regularisation stabilises convergence**: L2 regularisation particularly enhances MM performance and generalisability.  
- **Interpretability**: Model coefficients reveal important features such as payment history and borrower region, providing actionable insights for financial modelling.

---

## Repository Contents

- `notebooks/`
  - `thesis-logistic-mm.ipynb` : Main notebook with all experiments and analysis
- `data/`
  - `loan-data-preprocessed.npz` : Preprocessed LendingClub loan dataset
- `README.md` : This file

---

## Getting Started

1. **Open the notebook** in [Google Colab](https://colab.research.google.com/) or locally.  
2. Ensure the notebook has access to the preprocessed data: `data/loan-data-preprocessed.npz`.  
3. Run all cells sequentially to reproduce experiments, generate synthetic datasets, and analyse results.  

**No additional setup is required.** All code, data handling, and analysis are included in the notebook.

---

## Notebook Overview

| Section | Description |
|---------|-------------|
| Environment Setup | Imports and configuration for execution |
| Data Loading & Preparation | Loads preprocessed loan data and provides a synthetic data generator function |
| Optimisation Algorithms | Implements MM, GD, NR optimisers with support functions |
| Implementation | Experiment configurations, trial execution, logging |
| Analysis | Plots, convergence curves, feature importance, and synthetic dataset performance |

---

## Reproducibility

The notebook is fully self-contained:  

- Preprocessed real-world data is included (`loan-data-preprocessed.npz`).  
- Synthetic datasets are generated on-the-fly.  
- All metrics, convergence analyses, and plots can be reproduced by running the notebook cells.  
