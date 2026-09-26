# Questions Inbox

5. What objective function does K-Means minimize? Ans- K-Means minimizes the Within-Cluster Sum of Squares (WCSS), also called inertia. It is the sum of the squared distances between each data point and the centroid of its assigned cluster.

6. Why is feature scaling important in K-Means? Ans- K-Means relies on distance calculations, so features with larger numerical scales can dominate the distance. Scaling features ensures that variables with different units or ranges contribute more appropriately to cluster formation.

7. How do you choose the optimal value of K in K-Means? Ans- Common methods include the Elbow Method and Silhouette Analysis. The Elbow Method examines how WCSS decreases as K increases, while the Silhouette Score measures how well-separated and internally cohesive the resulting clusters are.

8. What is the Elbow Method in K-Means? Ans- The Elbow Method involves running K-Means with different values of K and plotting the corresponding WCSS. The point where the reduction in WCSS begins to slow significantly is considered a possible choice for K.

9. What is the Silhouette Score? Ans- The Silhouette Score measures how similar a data point is to its own cluster compared with the nearest other cluster. It ranges from -1 to 1, where a higher value generally indicates better-defined clustering.

10. Why is K-Means sensitive to initialization? Ans- K-Means can converge to different local optima depending on the initial centroid positions. Poor initialization can produce inferior clusters, which is why methods such as K-Means++ are commonly used to select better initial centroids.

11. What is K-Means++? Ans- K-Means++ is a centroid initialization method designed to select initial centroids that are well separated from one another. It generally provides better starting points than purely random initialization and can improve convergence and clustering results.

12. Why can K-Means produce different results on different runs? Ans- Different initial centroid positions can lead K-Means toward different local minima of its objective function. Using a fixed random_state makes the initialization reproducible, while multiple initializations can be used to search for a better solution.

13. What are the limitations of K-Means? Ans- K-Means requires the number of clusters to be specified, is sensitive to feature scaling and outliers, and generally works best when clusters are reasonably compact and separated. It may perform poorly for clusters with irregular shapes or very different densities.

14. How do outliers affect K-Means? Ans- Outliers can significantly shift cluster centroids because centroids are calculated using the mean. This can distort cluster boundaries and reduce clustering quality. Appropriate outlier handling or a more robust clustering method may be considered when outliers are substantial.

15. Why does K-Means struggle with non-spherical clusters? Ans- K-Means assigns points based on distance to centroids and minimizes squared Euclidean distances. This tends to favor compact, roughly spherical or convex clusters of comparable scale, making irregularly shaped clusters difficult to represent accurately.

16. What is the difference between K-Means and K-Medoids? Ans- K-Means represents each cluster using the mean of its points, while K-Medoids represents each cluster using an actual data point called a medoid. K-Medoids is generally more robust to outliers because the representative point is an existing observation rather than a mean.

17. Is K-Means guaranteed to find the global optimum? Ans- No. The standard K-Means algorithm is guaranteed to converge to a local optimum of its objective function, but it is not generally guaranteed to find the global optimum. Multiple initializations can improve the chance of obtaining a better solution.

18. How can you determine whether K-Means clustering is meaningful? Ans- Clustering quality can be evaluated using metrics such as Silhouette Score, Calinski-Harabasz Index, and Davies-Bouldin Index, along with visualization and domain-specific interpretation. A mathematically good clustering is not necessarily meaningful for the real-world problem.

19. What is the computational complexity of K-Means? Ans- For n data points, k clusters, d features, and i iterations, the typical time complexity is approximately O(nkdi). The actual runtime depends on the number of iterations, initialization strategy, implementation, and dataset characteristics.

20. What is the difference between K-Means and hierarchical clustering? Ans- K-Means directly partitions data into a predefined number of clusters by iteratively updating centroids, whereas hierarchical clustering builds a hierarchy of clusters that can be represented using a dendrogram. Hierarchical clustering does not necessarily require choosing the final number of clusters before constructing the hierarchy.
