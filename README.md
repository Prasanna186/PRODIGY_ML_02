Task-02: Create a K-means clustering algorithm to group customers of a retail store based on their purchase history.
K-means clustering is a popular unsupervised machine learning algorithm used for partitioning a dataset into a predetermined number of clusters. Here are the steps involved in the K-means clustering algorithm:

1. **Initialization**: Choose the number of clusters (K) and randomly initialize K cluster centroids. These centroids can be randomly selected data points or randomly generated within the range of the dataset.

2. **Assign Data Points to Clusters**: For each data point, calculate the distance to each centroid and assign it to the nearest centroid. Usually, Euclidean distance is used for this calculation.

3. **Update Cluster Centroids**: After assigning each data point to a cluster, recalculate the centroid of each cluster by taking the mean of all data points assigned to that cluster.

4. **Repeat**: Steps 2 and 3 are repeated iteratively until one of the stopping criteria is met. Common stopping criteria include:
   - Centroids do not change significantly between iterations.
   - Maximum number of iterations is reached.
   - Data points do not change clusters between iterations.

5. **Finalize Clusters**: Once the algorithm converges, the clusters are finalized, and each data point belongs to one cluster.

6. **Evaluate Clusters**: After clustering, you may evaluate the quality of clusters using various metrics such as silhouette score, Davies–Bouldin index, or within-cluster sum of squares (WCSS).

7. **Interpretation**: Finally, interpret the clusters and their centroids to gain insights into the structure of the data.

It's worth noting that K-means clustering is sensitive to the initial placement of centroids, and different initializations can lead to different clustering results. Therefore, it's common practice to run the algorithm multiple times with different initializations and choose the clustering with the lowest objective function value (e.g., the lowest WCSS).
