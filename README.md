# Customer Segmentation with Clustering Algorithms

## Overview
This project applies multiple clustering algorithms to customer segmentation, evaluating their effectiveness using silhouette scores and other performance metrics. The analysis highlights the strengths and weaknesses of K-Means, DBSCAN, Agglomerative Clustering, Spectral Clustering, and Affinity Propagation in identifying meaningful customer groups.

## Key Findings
- **K-Means Clustering** struggles to find an optimal number of clusters, suggesting the dataset lacks a strong natural clustering structure.
- **DBSCAN** effectively identifies core customer groups but is highly sensitive to noise, requiring significant data filtering.
- **Agglomerative Clustering** provides the best balance between silhouette score and cluster count, making it the most reliable choice for this dataset.
- **Spectral Clustering & Affinity Propagation** over-cluster the data, potentially leading to overfitting.

## Methodology
1. **Data Preprocessing**: Standardization and feature selection.
2. **K-Means Clustering**: Elbow method, silhouette analysis, and gap statistic to determine the optimal cluster count.
3. **DBSCAN**: Tuning `eps` to minimize noise while maximizing cluster structure.
4. **Agglomerative Clustering**: Evaluating linkage criteria and cluster compactness.
5. **Spectral Clustering & Affinity Propagation**: Comparison with other methods to assess overfitting risks.
6. **Model Evaluation**: Using silhouette scores to determine cluster quality.