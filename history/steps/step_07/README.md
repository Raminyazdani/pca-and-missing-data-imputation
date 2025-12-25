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
pca-and-missing-data-imputation/
├── code/
│   ├── pca_implementation.ipynb           # PCA implementation and analysis
│   ├── missing_data_imputation.ipynb      # Distribution-based imputation methods
│   ├── knn_imputation.ipynb               # k-Nearest Neighbor imputation
│   └── results/                           # Generated outputs (plots, metrics)
├── data/
│   ├── pca_toy.txt                        # PCA demonstration dataset
│   └── ms_toy.txt                         # Missing values demonstration dataset
├── requirements.txt
└── README.md
```

## Setup / Installation

```bash
pip install -r requirements.txt
```

## How to Run

Launch Jupyter from the repository root or code directory:

```bash
# From repository root
jupyter notebook

# Or from code directory
cd code
jupyter notebook
```

Then open any of the three notebooks:
- `pca_implementation.ipynb` - PCA implementation and variance analysis
- `missing_data_imputation.ipynb` - Distribution-based imputation methods
- `knn_imputation.ipynb` - k-Nearest Neighbor (kNN) imputation

## Data / Inputs

The project includes two toy datasets in the `data/` directory:
- `pca_toy.txt` - Tab-separated dataset for PCA demonstration (4 features, multiple samples)
- `ms_toy.txt` - Mass spectrometry dataset with missing values (NA) for imputation testing

Data files are accessed via relative paths from the notebooks (e.g., `../data/pca_toy.txt`).

## Outputs

Generated outputs are saved to the `code/results/` directory:
- **Principal components and variance explained** - Eigenvalues, eigenvectors, variance ratios
- **Imputed datasets with evaluation metrics** - RMSE and MAE for imputation quality
- **Visualizations**:
  - PCA scatter plots (PC1 vs PC2)
  - Imputation quality histograms and sweep plots
- **CSV files**:
  - `ctrl1_metrics_distribution.csv` - Distribution-based imputation metrics
  - `ctrl1_metrics_knn.csv` - kNN imputation metrics
  - `ctrl1_metrics_summary_min.csv` - Summary statistics

## Reproducibility Notes

- **Path handling**: All data paths are relative - notebooks expect data in `../data/` directory (accessible when running from `code/` directory or repository root)
- **Random seeds**: Set for reproducible results where applicable (e.g., in train/test splits and kNN)
- **Python version**: Tested with Python 3.x (3.8+)
- **Dependencies**: Install all requirements via `pip install -r requirements.txt`

## Troubleshooting

- **Path issues?** Ensure notebooks can access the `data/` directory. When running from `code/`, data is accessed via `../data/`. When running from repository root, ensure Jupyter's working directory allows relative path resolution.
- **Data not found?** Verify data files exist in the `data/` directory at repository root
- **Import errors?** Install dependencies: `pip install -r requirements.txt`
- **Module not found?** Ensure you have activated the correct Python environment

## Notes

This project demonstrates core statistical methods for data analysis:
- **PCA**: Eigendecomposition-based dimensionality reduction
- **Imputation**: Multiple strategies for handling missing data (distribution-based, kNN)
- **Validation**: Quantitative metrics (RMSE, MAE) and visual analysis
