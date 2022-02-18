# Cryptocurrencies
Cryptocurrencies using unsupervised machine learning

### Project Overview:

## Background:

A hypothetical investment bank is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked you to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.
The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.

## Purpose:

- Preprocessing the Data for PCA
- Reducing Data Dimensions Using PCA
- Clustering Cryptocurrencies Using K-means
- Visualizing Cryptocurrencies Results

## Resources: 

crypt_data.csv
https://min-api.cryptocompare.com/data/all/coinlist
https://min-api.cryptocompare.com/data/all/coinlist

Tools: 

Pandas, plotly.express, hvplot.pandas, sklearn.cluster library, sklearn library, PCA, StandardScalar library

## Analysis 

Unsupervised machine learning technique is used to discover patterns or groups in data since we don’t yet know the question we’re asking of the data.  

- First data is  pre-processed to remove unnecessary columns and rows with null values and strings data type is converted into numerical data.
- Then Standard Scalar is used to standardize the features.  Once the data is standardized, PCA is used to reduce the dimensions to 3 principal components. PCA model is fit and trained. 
= Then best number of centroids for K-Means is determined by plotting Elbow Curve. Since the elbow curve showed that 4 clusters will be most useful, K-Means model is created with 4 clustered and fitted and predictions are made.  

To visualize the results:
- Using Plotly Express and hvplot, a 3-d scatter plot is created with PCA data to visualize the distinct group that corresponds to the 3 principal components.  
- A table is created which shows all the currently tradeable cryptocurrencies 
- A scatter plot is created to visualize the TotalCoinSupply and TotalCoinsMined data after applying the Min_Max Scaler algorithm to scale the data between 0 and 1. 



