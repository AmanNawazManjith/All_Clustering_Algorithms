# Multiple_Clustering_Algorithms

## Clustering
Clustering is the task of dividing the population or data points into a number of groups such that data points in the same groups are more similar to other data points in the same group and dissimilar to the data points in other groups.

## Different Clustering Algorithms
```KMeans Clustering Algorithm```\
```Hierarchical Clustering Algorithm```\
```DBSCAN Clustering Algorithm```\
```Gaussian Mixture Algorithm```

## KMeans Clustering Algorithm

![image](https://user-images.githubusercontent.com/71788604/155832558-3d8e44b8-54e0-4aa3-948d-f1f9eeff4625.png)


The goal of the K-Means algorithm is to find clusters in the given input data. There are a couple of ways to accomplish this. A trial and error method is used by specifying the value of K (e.g., 3,4, 5). As we progress, we keep changing the value until we get the best clusters. \
Another method is to use the Elbow technique to determine the value of K. Once we get the K's value, the system will assign that many centroids randomly and measure the distance of each of the data points from these centroids. Accordingly, it assigns those points to the corresponding centroid from which the distance is minimum. So each data point will be assigned to the centroid, which is closest to it. Thereby we have a K number of initial clusters. For the newly formed clusters, it calculates the new centroid position. The position of the centroid moves compared to the randomly allocated one. Once again, the distance of each point is measured from this new centroid point. If required, the data points are relocated to the new centroids, and the mean position or the new centroid is calculated once again. If the centroid moves, the iteration continues indicating no convergence. But once the centroid stops moving (which means that the clustering process has converged), it will reflect the result.

## Hierarchical Clustering Algorithm

![image](https://user-images.githubusercontent.com/71788604/155832573-788db36c-053b-40d5-b565-c0032eb018de.png)


Hierarchical clustering, also known as hierarchical cluster analysis, is an algorithm that groups similar objects into groups called clusters. The endpoint is a set of clusters, where each cluster is distinct from each other cluster, and the objects within each cluster are broadly similar to each other.
A Hierarchical clustering method works via grouping data into a tree of clusters. Hierarchical clustering begins by treating every data points as a separate cluster. Then, it repeatedly executes the subsequent steps:
1.	Identify the 2 clusters which can be closest together, and
2.	Merge the 2 maximum comparable clusters. We need to continue these steps until all the clusters are merged together.
In Hierarchical Clustering, the aim is to produce a hierarchical series of nested clusters. A diagram called Dendrogram (A Dendrogram is a tree-like diagram that statistics the sequences of merges or splits) graphically represents this hierarchy and is an inverted tree that describes the order in which factors are merged (bottom-up view) or cluster are break up (top-down view).


## DBSCAN Clustering Algorithm

![image](https://user-images.githubusercontent.com/71788604/155832617-ae35bf0c-e9ac-4b36-b970-669d8c09d584.png)


DBSCAN - Density-Based Spatial Clustering of Applications with Noise. Finds core samples of high density and expands clusters from them. Good for data which contains clusters of similar density. \
What’s nice about DBSCAN is that you don’t have to specify the number of clusters to use it. All you need is a function to calculate the distance between values and some guidance for what amount of distance is considered “close”. DBSCAN also produces more reasonable results than k-means across a variety of different distributions.


## Gaussian Mixture Algorithm

![image](https://user-images.githubusercontent.com/71788604/155832642-2a8ca692-c882-445c-ac56-ea5fa974ffbe.png)


As the name implies, a Gaussian mixture model involves the mixture (i.e. superposition) of multiple Gaussian distributions.
Gaussian mixture models can be used to cluster unlabeled data in much the same way as k-means. But there are two main differences:

1.	First and foremost, k-means does not account for variance. By variance, we are referring to the width of the bell shape curve. (Standard Deviation of a Normal Distribution)
2.	The second difference between k-means and Gaussian mixture models is that the former performs hard classification whereas the latter performs soft classification. In other words, k-means tells us what data point belong to which cluster but won’t provide us with the probabilities that a given data point belongs to each of the possible cluster.



