# Questions Inbox

17. Is K-Means guaranteed to find the global optimum? Ans- No. The standard K-Means algorithm is guaranteed to converge to a local optimum of its objective function, but it is not generally guaranteed to find the global optimum. Multiple initializations can improve the chance of obtaining a better solution.

18. How can you determine whether K-Means clustering is meaningful? Ans- Clustering quality can be evaluated using metrics such as Silhouette Score, Calinski-Harabasz Index, and Davies-Bouldin Index, along with visualization and domain-specific interpretation. A mathematically good clustering is not necessarily meaningful for the real-world problem.

19. What is the computational complexity of K-Means? Ans- For n data points, k clusters, d features, and i iterations, the typical time complexity is approximately O(nkdi). The actual runtime depends on the number of iterations, initialization strategy, implementation, and dataset characteristics.

20. What is the difference between K-Means and hierarchical clustering? Ans- K-Means directly partitions data into a predefined number of clusters by iteratively updating centroids, whereas hierarchical clustering builds a hierarchy of clusters that can be represented using a dendrogram. Hierarchical clustering does not necessarily require choosing the final number of clusters before constructing the hierarchy.
