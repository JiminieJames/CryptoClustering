# CryptoClustering: Predicting Cryptocurrency Market Trends

## Project Overview

The **CryptoClustering** project applies unsupervised learning techniques to investigate the effects of short-term price changes on various cryptocurrencies. Utilizing K-means clustering and Principal Component Analysis (PCA), the project aims to uncover hidden patterns in the data, reduce its dimensionality, and provide insightful visualizations of clustering results.

## Table of Contents

- [About the Project](#about-the-project)
- [Data Preparation](#data-preparation)
- [Clustering Methodology](#clustering-methodology)
- [Dimensionality Reduction](#dimensionality-reduction)
- [Visualization and Analysis](#visualization-and-analysis)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## About the Project

Cryptocurrency markets are highly volatile, with significant price fluctuations occurring within short time frames. This project seeks to categorize cryptocurrencies based on their price changes over 24 hours and 7 days, applying K-means clustering both before and after reducing the data's dimensionality using PCA.

## Data Preparation

The data used in this project is sourced from `crypto_market_data.csv`. The dataset includes key metrics such as percentage changes in price over different time intervals, which serve as the basis for clustering.

### Key Steps in Data Preparation:

1. **Loading the Dataset:** Import the data from a CSV file and perform initial inspection.
2. **Preprocessing:** Handle missing values, if any, and scale the data to ensure that all features contribute equally to the analysis.
3. **Feature Selection:** Choose relevant features (e.g., price change percentages) for clustering.

## Clustering Methodology

### Finding the Optimal Number of Clusters

The optimal number of clusters (`k`) is determined using the elbow method, which helps identify the point where adding more clusters no longer significantly improves the variance explained.

### Applying K-means Clustering

K-means clustering is applied to the scaled dataset to categorize cryptocurrencies based on their price change behaviors.

## Dimensionality Reduction

### Principal Component Analysis (PCA)

PCA is employed to reduce the dataset to three principal components, capturing the most variance with the fewest dimensions. This step is crucial for visualizing high-dimensional data and improving the performance of clustering algorithms.

### Clustering on Reduced Data

K-means clustering is then reapplied to the PCA-transformed data, allowing for comparison between clustering results on original versus reduced data.

## Visualization and Analysis

### Comparison of Clustering Results

Scatter plots are generated to compare the clustering results before and after PCA. These visualizations provide insights into how dimensionality reduction affects the clustering of cryptocurrencies.

## Installation

To run this project, ensure you have the following dependencies installed:

- Python 3.x
- pandas
- NumPy
- scikit-learn
- hvPlot

## Usage

1. Run the Jupyter Notebook: Execute the notebook to preprocess data, find the optimal number of clusters, apply clustering algorithms, and visualize the results.
2. Modify Parameters: Experiment with different values of k or PCA components to observe how they impact the clustering results.

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to submit a pull request or open an issue.