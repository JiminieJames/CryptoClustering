# CryptoClustering
CryptoClustering

The Crypto Clustering project aims to predict if cryptocurrencies are affected by 24-hour or 7-day price changes using unsupervised learning techniques, specifically K-means clustering. Additionally, the project explores the impact of dimensionality reduction using Principal Component Analysis (PCA) on clustering.

# Project Title 

Cluster Crypto Currencies prices changes, Reduce dimensionality using PCA on Clustering.

## Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Installing](#installing)
- [Usage](#usage)
- [Contributing](#contributing)

## About

Data is provided in "crypto_market_data.csv" is provided in Resources section. 


## Getting Started

1. Run jupyter notebook file to upload data from cvs file
   
2. Cluster Data using K-Means Algorithm
   
3. Reduce dimensionality using PCA method


## Installing

install python packages: 

Python

pandas

NumPy

scikit-learn

hvPlot



## Usage

1. Load and preprocess the data.

2. Scale the data using StandardScaler.

3. Find the best value for k using the elbow method.

4. Cluster cryptocurrencies with K-means using the original scaled data.

5. Perform PCA to reduce the features to three principal components.

6. Find the best value for k using the PCA data.

7. Cluster cryptocurrencies with K-means using the PCA data.

8. Visualize and compare the results using hvPlot.


## Contributing

Contributors names: Mamatha Etikyala
