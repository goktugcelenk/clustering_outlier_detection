# Clustering and Outlier Detection

This project demonstrates **unsupervised clustering and anomaly detection** using classical machine learning algorithms.  
It applies **K-Means**, **DBSCAN**, and **Local Outlier Factor (LOF)** to identify structure and irregularities in tabular data.  
The analysis highlights how preprocessing, scaling, and algorithm choice influence cluster formation and detection of outliers.

---

## Overview

Clustering and anomaly detection are essential tools in exploratory data analysis.  
This notebook compares partition-based and density-based methods, showing how each interprets the same dataset:

| Algorithm | Type | Description |
|------------|------|-------------|
| **K-Means** | Partition-based | Divides data into compact, spherical clusters. Requires the number of clusters *k* in advance. |
| **DBSCAN** | Density-based | Groups points based on local density, automatically detecting noise and irregular samples. |
| **LOF** | Outlier detection | Scores data points by local deviation from their neighbors to identify anomalies. |

---

## Methods

- **Libraries:** `scikit-learn`, `pandas`, `NumPy`, `matplotlib`, `seaborn`
- **Preprocessing:** scaling with `MinMaxScaler` and `StandardScaler`
- **Evaluation metrics:**  
  - *Silhouette Score* — cluster separation and cohesion  
  - *Davies–Bouldin Index* — compactness and separation measure

---

## Results

The figure below shows clustering results obtained with **DBSCAN** (`eps = 0.15`, `min_samples = 5`).  
Two dense clusters are identified, while a few isolated samples are recognized as noise.  
This approach adapts to irregular shapes and densities, making it suitable for unsupervised anomaly detection tasks.

<img width="573" height="455" alt="image" src="https://github.com/user-attachments/assets/c2f8cf24-6b93-46c8-8a40-f8372379cf2d" />

---

## Learning Outcomes

- Understand differences between **partition-based** (K-Means) and **density-based** (DBSCAN) clustering.
- Apply **Local Outlier Factor (LOF)** for neighborhood-based anomaly detection.
- Use internal validation metrics to evaluate cluster quality.
- Visualize and interpret clustering results in two dimensions.

*This repository is part of a broader focus on unsupervised learning and data-driven anomaly detection within industrial analytics.*
