# Week 01 Log — Clustering (k-means) on Wine

## Date range
- 2026-01-14 to 2026-01-20
## What I worked on
- Implemented k-means clustering on the Wine dataset (sklearn built-in)
- Selected k using Elbow (WCSS) and Silhouette score
- Visualised clusters using PCA and interpreted clusters using feature means

## Resources used
- Lecture slides: Clustering / k-means / WCSS (Elbow) / Silhouette / PCA visualisation
- sklearn functions: load_wine, StandardScaler, KMeans, silhouette_score, PCA

## Dataset & preprocessing
- Dataset: Wine (178 samples, 13 numeric features)
- Missing values: none detected
- Scaling: StandardScaler (required because k-means is distance-based)

## Experiments & results
- k tested: 2..10
- Best k (silhouette): 3 (score ≈ 0.285)
- Outputs saved to `images/`:
  - week01_elbow_wcss.png
  - week01_silhouette_vs_k.png
  - week01_pca_clusters_k3.png
- Decision rationale: k=3 was chosen because it had the highest silhouette score (≈0.285) and the elbow curve starts to flatten around k≈3.
- Environment: VS Code + .venv (Python 3.13.7)
- Key interpretation features (largest differences across clusters):
  - proline, magnesium, color_intensity, alcalinity_of_ash, flavanoids
- Summary:
  - Cluster 0: lower proline/magnesium and much lower color_intensity
  - Cluster 1: highest color_intensity, very low flavanoids
  - Cluster 2: very high proline and high flavanoids

## Issues / fixes
- No major issues; ensured the notebook uses the project `.venv` interpreter and required packages were installed.

## Next steps
- Compare with hierarchical clustering (Agglomerative) using the same k
- Try a different dataset (e.g., customer segmentation) to test robustness
