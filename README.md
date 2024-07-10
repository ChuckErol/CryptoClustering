# CryptoClustering

## Overview:

- This project aims to use K-means clustering to categorize cryptocurrencies based on their price fluctuation patterns. By analyzing historical price data and using dimensionality reduction techniques, we hope to discover meaningful clusters that enhance market understanding and guide investment decisions. The project involves using both the original scaled dataset and applying PCA to reduce the dataset's dimensions, comparing the clustering results from each approach.

## Application K-Mean with original data:

- Imported and prepared cryptocurrency data from a CSV file.
- Normalized the data using scikit-learn's StandardScaler for improved clustering performance.
- Implemented the elbow curve method to determine the ideal number of clusters 'k' for K-means clustering. This involves iteratively calculating inertia for different k values and visually identifying the "elbow" in the resulting line chart (4 clusters seems to be the most opitmal for the model).
- Applied the K-means algorithm using the optimal k value obtained from the elbow curve method
- Grouped cryptocurrencies into distinct clusters based on their price change behavior.
- Visualize the clusters using hvPlot, highlighting data points with their corresponding cryptocurrency IDs for easy identification.

## Application K-Means with PCA scaled data:

- Performed PCA on the scaled data to reduce its dimensionality and potentially improve clustering results.
- Analyzed the explained variance of each principal component to assess the information retained after dimensionality reduction.
- Repeated the elbow curve method analysis using the PCA-transformed data to identify the best k value for this reduced dimensionality space.
- Compared the optimal 'k' obtained from the PCA data to the one found with the original data.
- Performed K-means clustering again, using the optimal k identified based on the PCA data.
- Grouped cryptocurrencies based on their principal components and visualize the resulting clusters using hvPlot.

## Sources:

- I found some of my codes from previous class activities.
- I ask some questions to my classmates in Slack and during our study group meeting.
- I found some helpful information watching various YouTube videos
- I found information from Leaflet documentation sections and Stack Overflow website.
