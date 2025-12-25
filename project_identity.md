# Project Identity

## Professional Identity
- **Display Title**: PCA and Missing Data Imputation
- **Repo Slug**: pca-and-missing-data-imputation
- **Tagline**: Statistical methods for dimensionality reduction and robust missing value estimation
- **GitHub Description**: Implementation of Principal Component Analysis (PCA) and multiple missing data imputation techniques for biological datasets, demonstrating dimensionality reduction and statistical approaches to incomplete data.
- **Primary Stack**: Python, Jupyter Notebook, NumPy, scikit-learn, Pandas
- **Topics/Keywords**: pca, missing-data-imputation, dimensionality-reduction, knn-imputation, statistical-methods, bioinformatics, data-science, machine-learning, python, jupyter-notebook, scikit-learn

## Problem & Approach
**Problem**: This project addresses two fundamental challenges in data analysis: reducing high-dimensional data to its most informative components via PCA, and handling missing values in datasets through various imputation strategies.

**Approach**: Implements PCA both from scratch and using scikit-learn, develops and compares multiple imputation algorithms (mean, median, k-Nearest Neighbors, iterative methods), validates results on toy datasets, and provides visualizations of principal components and imputation quality.

## Inputs & Outputs
**Inputs**:
- `pca_toy.txt` - Tab-separated dataset for PCA demonstration
- `ms_toy.txt` - Mass spectrometry toy dataset with missing values (NA)

**Outputs**:
- Principal component analysis results (variance explained, loadings)
- Imputed datasets with evaluation metrics (RMSE, MAE)
- Visualization plots (PCA scatter plots, imputation quality histograms)
- CSV files with imputation metrics and summaries
