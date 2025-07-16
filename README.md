## Clustering Case Study - Customer Segmentation with K-Means - Tier 3

## Date and Time
- Created/Updated: July 15, 2025, 06:59 PM PDT

## Overview
This Jupyter notebook implements a customer segmentation analysis using the `WineKMC.xlsx` dataset. It explores K-Means clustering with the Elbow and Silhouette Methods, visualizes results with PCA, and compares alternative clustering algorithms (Affinity Propagation, Spectral Clustering, Agglomerative Clustering, DBSCAN).

## Dataset
- **File**: `WineKMC.xlsx`
- **Sheets**:
  - `OfferInformation`: Details on 32 wine offers (e.g., varietal, discount, origin).
  - `Transactions`: Customer responses linked to offer IDs.
- **Size**: 100 customers, 32 features (binary offer responses).

## Exercises
1. **Data Wrangling**: Built a 100x32 customer-offer matrix.
2. **Elbow Method**: Identified K=3 as the optimal number of clusters.
3. **Silhouette Method**: Suggested K=9 (score 0.1466), peaking at K=10 (0.1508).
4. **PCA Visualization**: Plotted clusters in 2D (21.5% variance).
5. **Optimal Dimensions**: PCA elbow at ~13 dimensions (78.5% variance).
6. **Other Algorithms**: Compared performance, with Spectral Clustering best at K=3 (0.224).

## Results
- **Clustering Performance**:
  - Affinity Propagation: 15 clusters, 0.095
  - Spectral Clustering: 3 clusters, 0.224 (best)
  - Agglomerative Clustering: 3 clusters, 0.086
  - DBSCAN: 0 clusters, N/A
- **PCA**: 0.215 total variance explained in 2D.

## Interpretation
- Spectral Clustering outperforms due to its ability to capture non-linear patterns in sparse data.
- K=3 aligns with Elbow and Spectral results, offering clearer segmentation than K=9.

## Future Work
- Enhance features.
- Test higher PCA dimensions.
- Investigate additional clustering methods.

## Dependencies
- Python 3.x
- pandas, numpy, matplotlib, seaborn, scikit-learn

