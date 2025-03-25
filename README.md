# weight-maintenance-phenotyping

# 🧠 Weight Maintenance Phenotyping via UMAP Clustering

This repository provides a comprehensive machine learning pipeline to identify phenotypic clusters in individuals based on their weight loss and weight maintenance patterns. The analysis leverages multi-source behavioral and demographic data and applies deep learning-based dimensionality reduction and unsupervised clustering techniques to uncover behavioral phenotypes.

## 📌 Overview

The pipeline consists of the following major steps:

# 🧠 Weight Maintenance Phenotyping via UMAP Clustering

This repository provides a full pipeline for identifying behavioral phenotypes based on weight loss maintenance using deep learning and unsupervised clustering techniques. The analysis integrates dietary, physical activity, engagement, and demographic features to uncover meaningful subgroups using UMAP and KMeans.

---

## 📌 Overview

The workflow includes:

1. **Data Integration**
   - Merges data from SMART trial outputs, engagement logs, and analytic features.
   - Computes weight loss at months 3, 6, and 12.

2. **Outcome Labeling**
   - Binary label: Maintainer (1) if ≥5% weight loss at both Month 3 and Month 12, otherwise Non-maintainer (0).

3. **Feature Learning**
   - Trains a multi-layer perceptron (MLP) and extracts hidden layer activations as embeddings.

4. **Dimensionality Reduction**
   - Reduces embeddings to 2D using UMAP for visualization and clustering.

5. **Clustering and Evaluation**
   - Applies KMeans clustering on the UMAP space.
   - Evaluates optimal cluster number using Gap Statistic and Silhouette Score.

6. **Visualization**
   - Generates UMAP plots with convex hulls and group labels.
   - Highlights maintainers vs non-maintainers in 2D space.

7. **Phenotypic Characterization**
   - Z-scores cluster characteristics (e.g., activity, calorie/fat intake, engagement).
   - Outputs a clean summary of each cluster in Excel format.

---

## 📦 Dependencies

Key Python packages used:

numpy

pandas

scikit-learn

matplotlib

seaborn

xgboost

shap

umap-learn

bayesian-optimization

imbalanced-learn

pyreadr

scipy

Note: UMAP may require conda-based installation depending on your environment.



## 👨‍💻 Author
### Farzad Shahabi
PhD Candidate – Computer Science
Specializing in Mobile Health and Machine Learning
