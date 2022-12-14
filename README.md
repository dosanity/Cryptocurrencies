# Cryptocurrencies

## Project Overview

Cryptocurrency, sometimes called crypto-currency or crypto, is any form of currency that exists digitally or virtually and uses cryptography to secure transactions. Cryptocurrencies don't have a central issuing or regulating authority, instead using a decentralized system to record transactions and issue new units.
These currencies run on a distributed public ledger called blockchain, a record of all transactions updated and held by currency holders. Additionally, units of cryptocurrency are created through a process called mining, which involves using computer power to solve complicated mathematical problems that generate coins. Users can also buy the currencies from brokers, then store and spend them using cryptographic wallets.

We are tasked to create an analysis for clients who are preparing to get into the cryptocurrency market. Since there is no known output, we will be using unsupervised machine learning to help create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. To group the cryptocurrencies, we decided on a clustering algorithm and then use data visualizations to share our findings.

## Resources
+ Analysis Software: `Python 3.10`, `Jupyter Notebook 6.4.12`
+ Data Source: [CryptoCompare](https://min-api.cryptocompare.com/data/all/coinlist) - `crypto_data.csv`

## Results

### Elbow Curve
K-means is an unsupervised learning algorithm used to identify and solve clustering issues. K represents how many clusters there will be. These clusters are then determined by the means of all the points that will belong to the cluster. The K-means algorithm groups the data into K clusters, where belonging to a cluster is based on some similarity or distance measure to a centroid. An easy method for determining the best number for K is the elbow curve. Using inertia, we were able to determine that K = 4 is the ideal number for clustering.
![intra-cluster-distance](https://user-images.githubusercontent.com/29410712/207781619-f4ba645e-0674-4c6b-b440-f61671ba3f35.png)

### Tradable Cryptocurrencies
In our analysis, we determined there were 532 tradable cryptocurrencies.
![data-18-challenge-hvplot-table-showing-all-tradable-cryptocurrencies](https://user-images.githubusercontent.com/29410712/207773418-bf5bbd98-c35b-4a10-bfc3-ecbe095ec1a7.png)

### 3D Scatterplot
We created a 3D-Scatterplot with the PCA data and the clusters.
![crypto-pca-3D-1](https://user-images.githubusercontent.com/29410712/207781662-c7633eb5-d0d7-4ed2-9456-56c1c4f75acd.png)

![crypto-pca-3D-2](https://user-images.githubusercontent.com/29410712/207781687-979f46d9-caa0-4a36-84ae-9764e747895f.png)

### 2D Scatterplot
Additionally, we also created a 2D-Scatterplot with the PCA data and the clusters.
![data-18-challenge-hvplot-scatter-plot](https://user-images.githubusercontent.com/29410712/207773361-3f756bac-17ba-4c67-b12c-10246ecc645b.png)


