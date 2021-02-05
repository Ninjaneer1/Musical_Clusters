# Musical_Clusters
 implementation of clustering algorithms on Spotify music data

### Clustering Music Data.

The goal of this project is to experiment with clustering algorithms and determine a reasonable number of clusters in the data.
There is a goup of cells used to help sort through the dataset to pick out desired genres for making a subset of the data. The clustering algorithms do not produce well formed clusters from the entire dataset. It is better to work with a subset of the data, like a user's songlist, or a selection of songs from their favorite genres. This is something that a company selling music would be interested in for generating sales by suggesting music. Songs with similar characteristics to music they already listen to can be found within clusters formed by using algorithms using data unique to that user.

Dimensional Reduction is applied prior to applying clustering algorithms for comparison with clustering performed on the raw, non-reduced, data. For this I used PCA, and I also used UMAP. Of the two, I believe that UMAP had better performance.

I experimented with a few different algorithms starting with K-means. I moved on to experimenting with Gaussian Mixture next. Lastly, I briefly visited the effects of DBSCAN, but moved away from that method because I wanted to be able to assign a desired number of clusters as a parameter going into the process.

Libraries Used:
* pandas: used for working with Dataframes, and Series
* numpy: data computation and manipulation
* matplotlib: visualization
* seaborn: visualization
* scikit-learn: 
    * Clustering/Mixture: KMeans, GaussianMixture, DBSAN 
    * metrics: Silhouette
    * preprocessing: StandardScaler
    * model_selection: train_test_split

#### Possible Implementations:
    suggestion system for music sales or streaming service.

#### Future Work:
    Improved data implementation, create a dashboard, implement as plug-in to bigger system