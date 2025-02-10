# CryptoClustering
**Objective**: Predict if cryptocurrencies are affected by 24-hour or 7-day price changes using the K-Means algorithm, and explore how cluster analysis results differ when using scaled market data and applying Principal Component Analysis (PCA).

## Tools and Libraries
- Visual Studio Code
- Python
- Pandas
- Matplotlib
- hvPlot
- scikit-learn

## Setup and Usage
1. Clone this `CryptoClustering` repository to your local machine.
2. Navigate to the cloned directory in Visual Studio Code.
3. Open the Jupyter Notebook `Crypto_Clustering.ipynb`.
4. Run each cell sequentially for data preparation, finding the best value for `k`, clustering, PCA, and plotting the elbow curves and cluster scatter plots.

## Plots
The notebook analyzes data from the file `crypto_market_data.csv` in the `Resources` folder and generates the following plots:
- Elbow Curves: To determine the optimal number of clusters (best value for `k`).
  - `market_scaled_elbow_curve`: Based on the scaled market data DataFrame.
  - `pca_elbow_curve`: Based on the scaled PCA DataFrame.
- Cluster Scatter Plots: Shows how the cryptocurrencies are clustered.
  - `market_scaled_clusters`: Using 24-hour and 7-day price changes.
  - `pca_clusters`: Using principal components PC1 and PC2.

## Conclusions
This project demonstrates the impact of dimensionality reduction on cluster analysis results. It shows that reducing the number of features using PCA, while retaining the maximum variance in the original data, can enhance the clustering process.
