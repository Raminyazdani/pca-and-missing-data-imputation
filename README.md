# PCA and Missing Data Imputation Study

**Statistical methods for PCA and missing value estimation**

**Stack:** Python, Jupyter Notebook, NumPy, scikit-learn

## Overview

This project implements Principal Component Analysis (PCA) and missing data imputation techniques for biological data analysis. It demonstrates dimensionality reduction methods and statistical approaches for handling incomplete datasets—common challenges in bioinformatics and data science.

## Problem & Approach

**Problem:** Apply PCA for dimensionality reduction and implement robust methods for estimating missing values in biological datasets.

**Approach:**
- Implement PCA from scratch and using scikit-learn
- Develop missing data imputation algorithms
- Compare imputation strategies (mean, median, KNN, iterative)
- Validate results on toy datasets
- Visualize principal components and reconstructions

## Tech Stack

- Python 3.x - Core programming
- Jupyter Notebook - Interactive analysis
- NumPy - Numerical computations
- scikit-learn - ML algorithms and PCA
- Matplotlib - Visualization

## Folder Structure

```
Assignment_1_supplement/
├── code/
│   ├── assignment_1_1_1.ipynb    # PCA implementation part 1
│   ├── assignment_1_1_2.ipynb    # PCA implementation part 2
│   ├── assignment_1_2.ipynb      # Missing data imputation (kNN)
│   └── results/                   # Generated outputs (plots, metrics)
├── data/
│   ├── pca_toy.txt               # PCA demonstration dataset
│   └── ms_toy.txt                # Missing values demonstration dataset
├── requirements.txt
└── README.md
```

## Setup / Installation

```bash
pip install -r requirements.txt
```

## How to Run

Launch Jupyter from the code directory:

```bash
cd Assignment_1_supplement/code
jupyter notebook
```

Then open any of the three notebooks:
- `assignment_1_1_1.ipynb` - PCA implementation and variance analysis
- `assignment_1_1_2.ipynb` - Distribution-based imputation methods
- `assignment_1_2.ipynb` - k-Nearest Neighbor (kNN) imputation

## Data / Inputs

- `pca_toy.txt` - PCA demonstration dataset
- `ms_toy.txt` - Missing values demonstration dataset

## Outputs

- Principal components and variance explained
- Imputed datasets with evaluation metrics
- Visualization of dimensionality reduction
- Comparison of imputation methods

## Reproducibility Notes

- All data paths are relative: notebooks expect to run from the `code/` directory
- Data files accessed via `../data/` (will be migrated from `../Assignment_1_supplement/`)
- Random seeds set for reproducible results where applicable
- Originally created in an academic setting

## Troubleshooting

- **Path issues?** Ensure running notebooks from the `code/` directory
- **Data not found?** Verify data files exist in `../data/` (or legacy path `../Assignment_1_supplement/`)
- **Import errors?** Install dependencies: `pip install -r requirements.txt`

## Notes

- Originally created in an academic setting
- Three notebooks cover different PCA and imputation aspects
- Toy datasets included for demonstration
