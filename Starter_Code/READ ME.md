CryptoClustering Challenge

Overview
The CryptoClustering project is a deep dive into the world of cryptocurrencies, utilizing Python and unsupervised learning techniques to predict the impact of price changes over 24-hour and 7-day periods on various cryptocurrencies.


Data Analysis

- Conducted exploratory data analysis to understand the dataset.
- Standardized the data using `StandardScaler()` from scikit-learn.
- Created a new DataFrame with scaled data, maintaining `coin_id` as the index.

Determining the Best Value for k

- Implemented the elbow method to identify the optimal value for k.
- Plotted the elbow curve and documented the observation on the best value for k.

Clustering Cryptocurrencies with K-Means

- Applied K-means clustering to the original scaled data using the determined best value for k.
- Added the predicted cluster labels to the original dataset.
- Visualized the clusters using hvPlot to explore possible correlations.

Optimization with PCA

- Conducted Principal Component Analysis (PCA) to reduce the dimensionality of the data.
- Recorded the explained variance of the PCA components.
- Created a DataFrame with PCA data, setting `coin_id` as the index.

Clustering with PCA Data

- Repeated the elbow method with the PCA data to find the optimal k value.
- Clustered the cryptocurrencies using the PCA data.
- Visualized the clusters and interpreted the results.

Final Analysis

- Reflected on the impact of reducing features on the clustering using K-Means.
- Provided insights on how the PCA-optimized clusters compared with the original clusters.

Conclusion
The impact of using fewer features via PCA for K-Means clustering seems to be that it can lead to a clearer separation between clusters, since PCA is only trying to keep the most significant features that explain the majority of the variance in the data.

