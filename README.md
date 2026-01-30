# DSML_Portfolio
This repository contains week-by-week DSML portfolio work for Semester 2.

## Week 01 — Wine Dataset (k-means + kNN)

This week covers both **unsupervised** and **supervised** distance-based methods using the built-in Wine dataset (178 samples, 13 numeric features).  
For clustering, I applied **k-means** with **StandardScaler**, selected k using **Elbow (WCSS)** and **Silhouette score** (k=3), visualised clusters with **PCA**, and interpreted clusters via feature means.  
For classification, I implemented **kNN** with scaling, evaluated **k=1..20** using accuracy (and compared distance settings), and reported results with an accuracy curve and confusion matrix.

- **Project A — K-means clustering:** `Week01_Clustering_KMeans/`
- **Project B — kNN classification:** `Week01_kNN/`

## Week 02 — Breast Cancer Dataset (SVM + ANN)

This week explores two supervised learning approaches on the **Breast Cancer Wisconsin** dataset (binary classification: malignant vs benign).  
For **SVM**, I applied StandardScaler, compared **linear vs kernel** models (linear / RBF / polynomial), and tuned RBF hyperparameters (**C** and **gamma**) to select the best-performing setting (**RBF(C=1, gamma=0.01)**, accuracy ≈ **0.982**). Results are summarised using a kernel comparison plot and a confusion matrix.  
For **ANN**, I trained a simple feed-forward **MLP** classifier with scaling and compared activation functions (**logistic / tanh / relu**). In this run, all activations achieved the same accuracy (≈ **0.956**), and results are reported with an activation comparison plot and a confusion matrix.

- **Project A — SVM (kernel comparison + tuning):** `Week02_SVM_ANN/notebook/week02_svm.ipynb`
- **Project B — ANN/MLP (activation comparison):** `Week02_SVM_ANN/notebook/week02_ann.ipynb`
