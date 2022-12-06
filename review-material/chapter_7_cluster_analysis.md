# Cluster Analysis: Basic Concepts and Algorithms

## The purpose of the clustering:
1. Clustering for **understanding**: the clusters should capture the natural structure of the data
2. Clustering for **utility**: in the context of utility, cluster analysis is the study of techniques for finding the most representative cluster prototypes

## Different Types of Clusterings
> An entire collection of clusters is commonly referred to as a clustering
1. Hierarchical versus Partitional
2. Exclusive versus Overlapping versus Fuzzy
3. Complete versus Partial
   
## Different Types of Clusters
> Clustering aims to find useful groups of objects (clusters), where usefulness is defined by the goals of the data analysis. 
1. Well-Separated clusters
2. Prototype-Based clusters (center-based clusters)
3. Graph-Based (contiguity-based cluster): If the data is represented as a graph, where the nodes are objects and the links represent connections among objects, then a cluster can be defined as a connected component; i.e., a group of objects that are connected to one another, but that have no connection to objects outside the group. 

    An important example of graph-based clusters is a **contiguity-based cluster**, where two objects are connected only if they are **within** a specified distance of each other. This implies that each object in a contiguity-based cluster is closer to *some* other object in the cluster than to *any* point in a different cluster. 
4. Density-Based clusters
5. Shared-Property (Conceptual Clusters)
   
## K-means
1. K-means v.s. K-medoid
2. The Basic K-means Algorithm
3. Limits of Random Initialization: One technique that is commonly used to address the problem of choosing initial centroids is to **perform multiple runs**, each with a different set of randomly chosen initial centroids, and then select the set of clusters with the minimum sum of the squared error (SSE). 
4. K-means has difficulty detecting the “natural” clusters
> K-means objective function is a mismatch for “natural clusters we are trying to find because it is minimized by **globular clusters** of **equal size** and **density** or by clusters that are **well separated**.

<mark>K-means is restricted to data for which there is a notion of a **center** (centroid)</mark>
