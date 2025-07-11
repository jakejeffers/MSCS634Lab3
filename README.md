# Lab 3: Clustering with K-Means and K-Medoids on the Wine Dataset

**Author:** Jacob Jeffers  
**Course:** MSCS 634 – Data Mining  

## Overview
This lab focused on comparing two popular clustering techniques — K-Means and K-Medoids — using the Wine dataset from the `sklearn` library. The goal was to evaluate how well each method grouped the data and how closely those clusters aligned with the actual wine classes. I used metrics like Silhouette Score and Adjusted Rand Index (ARI) to measure clustering quality and also visualized the results using PCA for a clearer comparison.

## What I Did
- Loaded the Wine dataset and explored its features and class distribution
- Standardized the data using z-score normalization to ensure fair clustering
- Applied K-Means clustering with 3 clusters and recorded its Silhouette Score and ARI
- Applied K-Medoids clustering with 3 clusters and recorded the same metrics
- Visualized both clustering results using PCA-reduced scatter plots

## What I Noticed
- **K-Means** produced a Silhouette Score of **0.2975** and an ARI of **0.8972**
- **K-Medoids** gave a Silhouette Score of **0.2967** and an ARI of **0.8972**
- The ARI values were identical, showing that both methods grouped the data similarly when compared to the actual wine classes
- K-Means and K-Medoids both produced reasonable cluster separations, but K-Means had a slight edge in Silhouette Score and ran faster

## Challenges I Ran Into
Installing `scikit-learn-extra` for K-Medoids was the biggest hurdle. I initially ran into C++ build errors due to version mismatches and ended up creating a new virtual environment using Python 3.10, which resolved the issue. After that, everything ran smoothly. Visualizing the results with PCA helped bring the numbers to life and made it easier to compare the methods side by side.

## Files Included
- `lab3.ipynb`: The full Jupyter Notebook with code, output, and visualizations
- `README.md`: This summary of the lab and what I observed
