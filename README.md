# Types of clustering algorithms
When choosing a clustering algorithm, it's crucial to consider whether the algorithm scales to the target dataset and the desired characteristics of the clusters. An algorithm that scales linearly with the size of the target dataset would have its runtime decrease as compared with an algorithm that scales quadratically with the number of examples. Let's denote $n$ as the number of examples, $O(n)$ as the complexity of the linear-scaling algorithm, and $O(n^2)$ as the complexity of the quadratic-scaling algorithm. $O(n^2)$ algorithms are not practical and less effective than $O(n)$ algorithms when the number of examples are in millions. The desired characteristics or assumptions for forming clusters vary by each category of clustering techniques. Generally, they convey assumptions about the structure, distribution, and organization of the data, guiding the choice of clustering technique based on the dataset's expected properties.

Clustering techniques are basically categorized into four groups: centroid, density, distribution, and hierarchy.
## 1. Centroid-based Clustering
<p align="center">
<img src="https://developers.google.com/static/machine-learning/clustering/images/CentroidBasedClustering.svg" width="300" height="300">
</p>

This method identifies clusters by finding the center point, or centroid, of a group of data points. Clusters are formed based on the proximity of data points to the centroid, and each point is assigned to the cluster with the nearest centroid.

Centroid-based algorithms are efficient, effective, and simple but sensitive to initial conditions and outliers. They are efficient because these algorithms can process and cluster data relatively quickly. They are effective because they produce meaningful and accurate clustering results. They are simple because they don't involve complex calculations or intricate procedures. That makes them easy to understand, implement, and use. Centroid-based clustering, such as K-means, has its strengths and weaknesses.

Pros:
- Simplicity and Speed: These methods are computationally efficient and easy to implement, making them suitable for large datasets.
- Scalability: They often perform well on high-dimensional data and can scale to a large number of data points
- Convergence: The algorithm usually converges quickly to a solution, providing a relatively fast clustering process.
- Well-suited for Balanced Clusters: They work well when clusters are spherical and of similar size
  
Cons:
- Sensitivity to Initialization: K-means, in particular, is sensitive to the initial placement of centroids, which can result in different clusters.
- Assumes Circular Clusters: K-means assumes that clusters are spherical and equally sized, which may not reflect the true nature of all datasets.
- Outliers Impact Results: The presence of outliers can significantly affect the centroid positions and, consequently, the clustering results.
- Fixed Number of Clusters: The user must specify the number of clusters beforehand, which might not be known in real-world scenarios.

In summary, centroid-based clustering is a powerful and efficient approach, especially for well-behaved datasets. However, it may struggle with more complex data structures and is sensitive to certain parameters and assumptions

## 2. Density-based Clustering
<p align="center">
<img src="https://developers.google.com/static/machine-learning/clustering/images/DensityClustering.svg" width="300" height="300">
</p>




## 3. Distribution-based Clustering
<p align="center">
<img src="https://developers.google.com/static/machine-learning/clustering/images/DistributionClustering.svg" width="300" height="300">
</p>

## 4. Hierarchical Clustering
<p align="center">
<img src="https://developers.google.com/static/machine-learning/clustering/images/HierarchicalClustering.svg" width="500" height="500">
</p>


Note: Source of images from [google](https://developers.google.com/machine-learning/clustering/clustering-algorithms)
