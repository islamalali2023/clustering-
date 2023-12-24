Model	Normalization	Standardization
Kmeans     	0.23137	0.26262
Goussian	  0.45202	0.46006
Bdscan	    0.00127	-
Spectral  	Model crashed
Minibatch	-	0.20147
Agglomerative	Model crashed
Clarans	    Running for long time then crashed
britch	    Model crashed

Clustering report:
1.	Check for correlation between features. 
2.	From data description: min-max variation suggests that normalization or scaling may be necessary before performing clustering.
3.	Normalization for data (min-max range =0-1 because data large difference between min and max (This helps to ensure that all features contribute equally to the distance computations performed by clustering algorithms).

4.	Rely on variance: Features with higher variance might be more influential in the clustering process.
5.	PCA: step to reduce the dimensionality of the data while retaining as much variance as possible.
6.	K-elbow: decide number of clusters (6 clusters).
7.	Silhouette: indicate that value close to zero means clusters are overlapped (0.0424, 0.035) for normalization and standardization respectively. 
8.	Result: the best result I got is doing clustering using GMM and my score is 0.46. 

