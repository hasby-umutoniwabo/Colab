# PCA: African Economic Crisis Data

## Overview
Principal Component Analysis (PCA) implementation from scratch using NumPy on the Africa Economic, Banking and Systemic Crisis Dataset (1860-2014, 13 African countries).

## Tasks
- **Task 1**: PCA from scratch (standardization, covariance, eigendecomposition, projection)
- **Task 2**: Dynamic component selection based on explained variance threshold
- **Task 3**: Performance benchmarking across dataset sizes and feature counts

## Dataset
- **Source**: [Kaggle - Africa Economic Crisis Data](https://www.kaggle.com/datasets/chirin/africa-economic-banking-and-systemic-crisis-data)
- **Shape**: 1059 rows × 14 columns
- **Non-numeric columns**: cc3, country, banking_crisis

## Installation & Usage

### Requirements
- Python 3.x
- Google Colab (recommended)

### Run in Google Colab
1. Open the notebook file (`PCA_Formative.ipynb`) in Google Colab
2. Click **Runtime → Run all**
3. The first cell installs `kagglehub` and downloads the dataset automatically

### Run Locally
```bash
pip install numpy pandas matplotlib kagglehub
jupyter notebook PCA_Formative.ipynb
```

## Results
- 9 components needed for 90% variance retention
- Compression ratio: 1.4x (13 → 9 features)
- Runtime: O(n·d²)
