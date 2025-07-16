README - Wine Customer Segmentation Project
==========================================

Date: July 15, 2025
Time: 06:59 PM PDT

Overview
--------
This project analyzes a dataset of 100 customers' responses to 32 exclusive wine offers to perform customer segmentation using clustering algorithms. The dataset, stored in "WineKMC.xlsx," includes offer details (e.g., varietal, discount, origin) and transaction data. The goal is to identify natural customer groups for targeted marketing strategies.

Files
-----
- WineKMC.xlsx: Contains two sheets - "OfferInformation" and "Transactions" with customer and offer data.
- Clustering Case Study - Customer Segmentation with K-Means - Tier 3.ipynb: Jupyter notebook with code and analysis.

Methodology
-----------
- Data Wrangling: Created a customer-offer matrix (100x32) using pandas pivot_table.
- Clustering: Applied K-Means, Affinity Propagation, Spectral Clustering, Agglomerative Clustering, and DBSCAN.
- Evaluation: Used Elbow Method, Silhouette Score, and PCA for dimensionality reduction and visualization.
- Optimal K: Silhouette Method suggested K=9 (score 0.1466), while Elbow Method and Spectral Clustering favored K=3 (score 0.224).

Results
-------
- Best Algorithm: Spectral Clustering (3 clusters, Silhouette Score 0.224).
- PCA Variance: 21.5% explained in 2D, indicating limited representation.
- Challenges: Sparse, high-dimensional data led to weak clustering structure.

Next Steps
----------
- Feature engineering.
- Test higher dimensions.
- Explore additional algorithms.
