# Cluster-Analysis
Dataset: Wolberg,WIlliam. (1992). Breast Cancer Wisconsin (Original). UCI Machine Learning 
<br>
Repository. https://doi.org/10.24432/C5HP4Z.

## K-means Clustering in Data Analysis

### What is K-means Clustering?

**K-means clustering** is one of the simplest and most widely used **unsupervised machine learning** algorithms. It is a method used in data analysis to divide a set of data points into distinct groups, or clusters, based on their similarities. The main goal of K-means is to find natural groupings in the data and to assign each data point to the most appropriate cluster. 

The K-means algorithm works iteratively and follows a few key steps to converge on the best result:

### Steps in K-means Clustering

#### Step 1: Defining the Number of Clusters (K)
The first step is to determine how many clusters you want the algorithm to produce. The number of clusters, denoted as **'k'**, represents the centroids you need to find within the dataset. Choosing the right 'k' value is crucial and can depend on domain knowledge or methods like the elbow method.

#### Step 2: Initializing the Centroids
Next, initialize **'k' centroids**. These centroids can either be chosen randomly or based on prior knowledge. These initial centroids are what the data points will be grouped around.

#### Step 3: Assigning Data Points to the Nearest Centroid
Once the centroids are initialized, the algorithm assigns each data point to the **closest centroid** based on a distance measure, like **Euclidean distance**. All data points that are close to a particular centroid are grouped into that cluster.

#### Step 4: Recalculating the Centroids
After the initial assignment of data points to clusters, the **centroids** are recalculated. The new centroid is found by calculating the **mean (average)** of all data points within that particular cluster. This becomes the new center of the cluster.

#### Step 5: Repeating the Assignment and Update Process
The assignment of data points to the nearest centroid and recalculation of the centroids is repeated iteratively. After each iteration, the centroids may shift based on the new cluster assignments. The algorithm continues until the centroids converge, meaning they no longer move significantly.

#### Step 6: Final Clusters
After the centroids have stabilized and no longer shift significantly, the algorithm concludes. At this point, the data points are grouped into **'k' distinct clusters**, with each cluster represented by its centroid.

### In Summary:
K-means clustering works by **iteratively** identifying **'k' centroids**, assigning each data point to the **nearest centroid**, recalculating the centroids based on the new groupings, and repeating this process until convergence. The result is that each data point belongs to the cluster nearest its centroid, and the cluster itself is represented by that centroid. 

The term "K-means" comes from the **means** (average) used to calculate the centroid location within each cluster. This method is a powerful way to identify inherent groupings in datasets, especially when the relationships within the data are unknown or too complex for traditional classification techniques.

### K-means and Our Analysis
In this project, K-means clustering was employed as part of our **SAS Enterprise Miner** workflow to classify data points into meaningful groups based on similarities. These clusters were then analyzed and further examined to help guide strategic insights for decision-making.

---

