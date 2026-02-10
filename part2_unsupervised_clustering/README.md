# Part 2 – Unsupervised Learning (Clustering with DBSCAN)

## Goal
Evaluate the effectiveness of density-based clustering using the DBSCAN
algorithm on multiple datasets with different structural properties.

The goal is to analyze how data density, noise, and cluster shape
affect clustering performance and stability.

## Workflow
- Data preprocessing and scaling
- DBSCAN hyperparameter selection (`eps`, `min_samples`)
- Clustering evaluation using internal metrics
- Dimensionality reduction (PCA / t-SNE) for visualization
- Comparative analysis across datasets

## Algorithm Choice
DBSCAN was selected due to its ability to:
- Detect arbitrarily shaped clusters
- Identify noise and outliers explicitly
- Operate without predefining the number of clusters

These properties make it suitable for datasets with unknown structure.

## Evaluation
Clustering quality is evaluated using:
- Silhouette score
- Additional internal clustering metrics

Metric behavior is analyzed in relation to dataset characteristics.

## Key Insights
- Clustering quality is highly sensitive to the `eps` parameter
- Different datasets require different density assumptions
- DBSCAN performs well on clearly separated dense regions, but
  struggles with varying cluster densities

## Notebook
Full implementation and analysis:
`notebooks/part2_unsupervised_clustering.ipynb`
