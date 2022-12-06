## Question 1.
a. Using the single link (MIN) hierarchical clustering technique, which pair of groups would you 
consider for merging? Provide a one-sentence justification. 

**Group A and Group B**,  define d(A,B) as group A and group B's minimum distance between each element of the cluster A and each element of the cluster B. d(A,B) < d(A,C) < d(B,C)>

b. Using the complete link (MAX) hierarchical clustering technique, which pair of groups would you consider for merging? Provide a one-sentence justification.  

**Group A and Group C**, define d(A, C) as group A and group C's maximum distance between each element of the cluster A and each element of the cluster C. d(A,C) < d(B, C) < d(A,C)>

## Question 2.
a) EPS = 0.4:  
b) EPS=1:  
## Question 3.
No, it is not necessary that SSE will also judge C1 to be a more accurate clustering than C2. Entropy is the degree to which each cluster consists of objects of a single class. SSE is the sum of the squared differences between each observation and its group's mean. Unlike entroty, SSE can be used as a measure of variation within a cluster. 
## Question 4. 

| Set of Points  | Similarity Matrix |
|----------------|-------------------|
| 1              |           A       |
| 2              |     C             |
| 3              |         D         |
| 4              |       B           |
## Question 5.
a) State two similarities and two differences between SNN density-based clustering and DENCLUE. 

similarities:
1. density-based clustering
2. unsupervised clustering

differences:
1.  DENCLUE utilizes a global density measure, SNN density-based clustering utilizes a local density measure.
2.  DENCLUE defines a point's density using a kernel function, whereas SNN density-based clustering employs a distance-based measure.
 
b) Explain two major advantages of Chameleon over hierarchical clustering using group average. 

1. Using using group average, Chameleon find clusters in a dataset more quickly than hierarchical clustering. 
2. Using using group average, Chameleon handles datasets with varying densities and shapes so it is more robust than hierarchical clustering. 
 
c) Whenever two clusters, C1 and C2, produced by standard K-means clustering are merged and the new 
centroid is computed as in K-means, the resulting SSE after merging is always greater than or equal 
to the SSE of the two clusters before merging. True or False? Explain briefly. 

False. It depends on the distance between the new centroid after merging and the data points. 

## Question 6.
a) Note that the noise is included in the two clusters. 

* Center-based: 2 clusters. left side of the rectangular and right side of the rectangular. 
* Contiguity-based: 1 cluster. Noise can be seen as a bridge between two circles. 
* Density-based: 2 clusters. 2 circles. 
 
b) The dots form multiple lines. 

* Center-based: 2 clusters. left group and right group of dot lines. 
* Contiguity-based: 5 clusters. Each dot line is a cluster.
* Density-based:  2 clusters. left group and right group of dot lines, in between is a low density region. 

## Question 7.
a)  By visual inspection, which two points would you consider as the outliers: A, B, C or D?  

A and B
 
b)  Assume that you are asked to use the kth nearest neighbor method to detect outliers with k = 1. Which 
two points would you consider as the outliers: A, B, C, or D?

B and D

c)  Assume that you are asked to use the LOF method to detect outliers. Which two points would you 
consider as the outliers: A, B, C, or D? 

A and B

d)  Based on your answers to questions (a)-(c), what can you say about the relative performance of the 
distance to the kth-nearest neighbor and LOF algorithms? 


LOF algorithms has better performance than kth-nearest neighbor, since it is based on local density. 

## Question 8.
Since we use a clustering-based approach to find anomalies in which the data is clustered using K-means, it is challenging to identify anomalies. For (a), the anomaly is easier to be dected than (b) since other three clusters in (a) are more similar with each other. For (b), since the clusters all have varying size, the anomaly is harder to de detected. 