# Finding-Gene-Variants-from-Sequencing-Data
Bioinformatics, Python

Finding gene variants is important in many areas of biology, including evolution and disease 
research.  
In this project, we focus on identifying gene variants from large batches of sequenced data. 
A single sample may contain numerous variants of the same gene. We are experimenting 
with multiple clustering algorithms with a goal to group similar reads together based on 
their sequence similarity. Each group, or cluster, represents one gene variant, whereas the 
representative sequence (centroid) is used as the final form of that variant.  
To handle this large amount of data, we picked HDBSCAN (Hierarchical Density-Based 
Spatial Clustering of Applications with Noise) and K-Means as our clustering algorithms. 
HDBSCAN is a clustering algorithm that groups similar data points based on how close and 
dense they are, without needing to know the number of clusters in advance. It can also 
identify and separate out noise or outliers automatically. 
K-Means, on the other hand, separates samples into a predefined number of clusters by 
minimizing the sum of squared distances between each point and the center of its 
assigned cluster. 
We ensure that only representative sequences are aligned for testing where we use 
pairwise alignment.  
In the following section, we describe the practical implementation of our approaches, 
including data preparation, clustering and sequence comparison.
