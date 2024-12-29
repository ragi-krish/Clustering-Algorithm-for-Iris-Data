# Clustering-Algorithm-for-Iris-Data

**Objective**

The objective of this project is to evaluate the understanding and application of clustering techniques using the Iris dataset. The project involves implementing and analyzing two clustering algorithms: KMeans Clustering and Hierarchical Clustering.

-----
**Dataset**

The Iris dataset, available in the sklearn library, is used for this project. This dataset contains measurements for four features (sepal length, sepal width, petal length, petal width) of three species of Iris flowers.

Since this is a clustering problem, the species column is dropped, leaving only the feature columns for analysis.

-----
**Key Components**

**1. Loading and Preprocessing** 

- The Iris dataset was loaded from the sklearn library.
- The species column was dropped to focus on unsupervised clustering techniques.

**2. Clustering Algorithm Implementation** 

**A) KMeans Clustering** 

1. **Description**:
   1. KMeans clustering is a partition-based clustering technique that groups data into a pre-defined number of clusters (k). It minimizes the variance within each cluster.
   1. The algorithm iteratively assigns data points to clusters based on the shortest Euclidean distance to the cluster centers and updates the cluster centers.
1. **Suitability for the Iris Dataset**:
   1. KMeans is suitable for the Iris dataset because it is effective for well-separated clusters, and the dataset's features provide clear distinctions among clusters.
1. **Implementation**:
   1. Applied KMeans clustering to the preprocessed Iris dataset.
   1. Visualized the clusters using 2D and 3D scatter plots.

**B) Hierarchical Clustering** 

1. **Description**:
   1. Hierarchical clustering builds a tree-like structure (dendrogram) by recursively merging or splitting clusters.
   1. Two main approaches:
      1. **Agglomerative**: Start with each data point as its own cluster and merge them.
      1. **Divisive**: Start with all points in one cluster and split them.
1. **Suitability for the Iris Dataset**:
   1. Hierarchical clustering is suitable for the Iris dataset because it provides insights into the hierarchical relationships among data points, which can be useful for exploratory analysis.
1. **Implementation**:
   1. Applied Agglomerative Hierarchical clustering to the preprocessed Iris dataset.
   1. Visualized the clusters using dendrograms and scatter plots.
-----
**Visualizations**

- Scatter plots for KMeans clusters.
- Dendrogram for Hierarchical clustering.
- Comparison of clustering results.
-----
**Results**

- KMeans clustering successfully identified distinct clusters in the dataset.
- Both clustering methods effectively identified the natural grouping in the Iris dataset. The consistent silhouette score of 0.7814 suggests that both algorithms performed equally well, capturing the intrinsic structure of the data.
- Hierarchical clustering provided a hierarchical structure, visualized through a dendrogram, showing relationships between data points.

