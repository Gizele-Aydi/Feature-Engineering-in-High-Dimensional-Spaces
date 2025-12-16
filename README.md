# Feature-Engineering-in-High-Dimensional-Spaces
This project explores feature engineering techniques for high-dimensional, sparse, and noisy datasets, using the Golub ALL/AML gene expression dataset as a case study. The goal is to identify, reduce, and transform relevant features to improve machine learning model performance.
# Feature Engineering in High-Dimensional Genomic Data
---

## Key Features

- **Supervised Feature Selection**
  - Mutual Information
  - L1 Regularization (Lasso)
  - Elastic Net (optional)
  
- **Dimensionality Reduction / Representation Learning**
  - Principal Component Analysis (PCA)
  - Kernel PCA (non-linear)
  - Non-negative Matrix Factorization (NMF)
  - Neural representations (future extension)

- **Model-Dependent Feature Importance**
  - Random Forest to rank predictive genes

- **Benchmarking**
  - Compare supervised vs. unsupervised techniques
  - Evaluate downstream performance using cross-validated Random Forest classifiers

- **Visualization**
  - Scree plots, PCA/KPCA scatter plots
  - NMF latent space plots
  - Feature importance bar plots

---

## Purpose

- Demonstrate how **feature engineering improves model interpretability and performance** in high-dimensional genomics datasets.
- Provide a **reproducible workflow** for preprocessing, selecting, and transforming features.
- Serve as a reference for applying feature engineering techniques in **bioinformatics, NLP, and other high-dimensional domains**.

---

## Installation

Clone this repository:

```bash
git clone https://github.com/yourusername/high-dimensional-feature-engineering.git
cd high-dimensional-feature-engineering
```
## Install dependencies (recommended to use a virtual environment):

```bash
pip install -r requirements.txt
```
## Usage

Place the Golub ALL/AML dataset (dataset_ALL_AML_train.csv) in the project directory.

Run the Jupyter notebook feature_engineering.ipynb to reproduce all preprocessing, feature engineering, visualization, and benchmarking steps.

Explore supervised selection, dimensionality reduction, and model-dependent techniques.

Benchmark different techniques using cross-validated Random Forest classification.

## Results

Supervised Feature Selection achieved the highest classification accuracy (~87%) on the ALL/AML dataset.

Dimensionality Reduction (PCA, Kernel PCA, NMF) is effective for visualization and capturing latent patterns but slightly underperforms supervised selection.

Random Forest Feature Importance highlights top predictive genes, complementing feature selection and dimensionality reduction insights.

Visualizations include scatter plots of PCA/KPCA/NMF components and feature importance bar plots.

## License

This project is licensed under the MIT License.
