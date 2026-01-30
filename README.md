# DSML_Portfolio
This repository contains week-by-week DSML portfolio work for Semester 2.

## Week 01 — Wine Dataset (k-means + kNN)

This week covers both **unsupervised** and **supervised** distance-based methods using the built-in Wine dataset (178 samples, 13 numeric features).  
For clustering, I applied **k-means** with **StandardScaler**, selected k using **Elbow (WCSS)** and **Silhouette score** (k=3), visualised clusters with **PCA**, and interpreted clusters via feature means.  
For classification, I implemented **kNN** with scaling, evaluated **k=1..20** using accuracy (and compared distance settings), and reported results with an accuracy curve and confusion matrix.

- **Project A — K-means clustering:** `Week01_Clustering_KMeans/`
- **Project B — kNN classification:** `Week01_kNN/`
