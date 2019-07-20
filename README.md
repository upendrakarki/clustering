# Clustering  
Clustering is basically a technique that groups similar data points such that the points in the same group are more similar to each other than the points in the other groups. The group of similar data points is called a Cluster.  

#Data Cleaning  
Replace null value with the mean for all the column containing null values  
Normalize the dataset before performing any Clustering algorithm  
  
# DBSCAN  
Density-based spatial clustering of applications with noise (DBSCAN)   
Based on a set of points, DBSCAN groups together points that are close to each other based on a distance measurement and a minimum number of points. It also marks as outliers the points that are in low-density regions.  
PARAMETERS-->    
eps=0.3 -- how close points should be to each other to be considered a part of a cluster    
min_samples=10 -- the minimum number of points to form a dense region  


# Hierarchical Clustering  
This clustering technique is divided into two types:  
1. Agglomerative  
2. Divisive  

The basic algorithm of Agglomerative is straight forward.  
- Compute the proximity matrix  
- Let each data point be a cluster  
- Repeat: Merge the two closest clusters and update the proximity matrix  
- Until only a single cluster remains   
  
The Hierarchical clustering Technique can be visualized using a Dendrogram.  
A Dendrogram is a tree-like diagram that records the sequences of merges or splits.  

PARAMETERS-->  
n_clusters=7 -- The number of clusters to find. It must be None if distance_threshold is not None    
affinity='euclidean' -- Metric used to compute the linkage
linkage='ward' --  The linkage criterion determines which distance to use between sets of observation  
