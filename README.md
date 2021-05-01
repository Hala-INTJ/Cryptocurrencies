# Challenge 18: Cryptocurrencies

## Overview of Cryptocurrencies

This project will use the unsupervised learning to cluster and plot information in relation to a number of cryptocurrencies. The available cryptocurrency data is not ideal, therefore, the following steps were applied:
- Removed all cryptocurrencies that are not being traded and which did not have a working algorithm
- Removed all records that had at least 1 null value
- Removed all records with no coins mined
- Converted text columns - "Algorithm" and "ProofType" - to binary values using pd.get_dummies
- Prepared the data for clustering by applying standard scaling (StandardScaler)
- Used Principal Component Analysis (PCA) to reduce dimensions to the most significant three principal components
- Identified the optimal number of clusters using elbow curve
- Used K-Means to classify the cryptocurrencies into four clusters
- Created a 3D scatter plot of the clustered cryptocurrencies
- Indicated the resulting number of tradable cryptocurrencies
- Normalized the "TotalCoinSupply" and "TotalCoinsMined" using MinMaxScaler
- Created a final two-dimensional scatter plot, "TotalCoinsMined" vs "TotalCoinSupply"


One key observation from both scatter plots indicated that "BitTorrent" was distinguished quite clearly from all other cryptocurrencies. 

