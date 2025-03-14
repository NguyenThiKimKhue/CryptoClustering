# CryptoClustering

Overview:
This assignment focuses on clustering cryptocurrencies using K-means and Principal Component Analysis (PCA) on market data. The goal is to explore, normalize, and determine the optimal number of clusters.

Data: csv file

Data Preparation
  1.	Normalization: Use StandardScaler() to normalize the data. Create a new DataFrame with the scaled data, setting "coin_id" as the index.
  2.	Output: Display the first five rows of the scaled DataFrame.
   
Finding the Best Value for k - Elbow Method:
  Clustering with K-means
  1.	K-means Implementation:
  o	Initialize and fit the K-means model using the scaled DataFrame.
  o	Predict clusters and update the DataFrame with these predictions.
  2.	Visualization: Create a scatter plot using hvPlot with "price_change_percentage_24h" vs. "price_change_percentage_7d".
   
Optimize Clusters with PCA
  1.	PCA: Reduce features to three principal components and retrieve the explained variance.
  2.	Output: Display the first five rows of the PCA DataFrame.
   
Finding the Best Value for k using PCA
  1.	Elbow Method on PCA: Repeat the elbow method and plot the results.
  2.	Analysis: Document the best k value and compare it with the previous k value.
   
Clustering with K-means on PCA
  1.	K-means with PCA: Fit the K-means model using the PCA DataFrame and predict clusters.
  2.	Visualization: Create a scatter plot with "PC1" vs. "PC2".
  3.	Impact Analysis: Discuss the effect of using fewer features for clustering.

Prepared by Kim Nguyen
