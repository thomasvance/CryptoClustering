# CryptoClustering

Analysis of Clustering Results Using PCA and Original Data
Overview of Data
The data consists of two main sources: PCA (Principal Component Analysis) transformed data and the original data. Each dataset includes two principal components, referred to as PCA1 and PCA2, which serve as the primary features for clustering. The crypto_segment column indicates the clustering category for each cryptocurrency, while the coin_id serves as an identifier for each coin.

Clustering with K-Means
K-Means clustering is a popular method used to partition data into distinct groups based on feature similarities. In this analysis, we have explored the performance of K-Means clustering using both the original data and the PCA-transformed data.

Optimal Number of Clusters (k):<br>
![Screenshot 2024-11-03 112126](https://github.com/user-attachments/assets/50fa3ea1-4132-4d37-b9d1-04a478a20026)

For the original data, the best value for k was determined to be 4.
For the PCA data, the optimal k was found to be 3.
This change in the optimal number of clusters highlights the impact of dimensionality reduction, as PCA simplifies the data by capturing the most variance with fewer features.
Explained Variance:

The explained variance for the PCA components indicates how much information is retained after transformation. The first two components together explain a significant portion of the total variance, which suggests that the dimensionality reduction was effective in preserving the essential characteristics of the data.
Visual Analysis:

The scatter plots comparing PCA and original data reveal distinct clustering patterns. The PCA data clusters more tightly, which may suggest that dimensionality reduction helps emphasize the relationships among cryptocurrencies, potentially leading to more coherent groupings.
In contrast, the original data may exhibit a broader distribution, indicating that additional features (dimensions) might introduce noise or complexity that obscures meaningful patterns.
Impact of Using Fewer Features
The analysis shows that using fewer features through PCA can lead to:

Simplified Models: With fewer dimensions, the clustering model may be less prone to overfitting and more interpretable.
Enhanced Performance: Clustering results using PCA often yield tighter clusters, which can improve the quality of insights drawn from the analysis.
Focus on Key Relationships: PCA highlights the most significant variance in the data, allowing for better identification of intrinsic groupings that might not be apparent when using a larger set of features.
Conclusion
The results of this analysis demonstrate the utility of PCA in preparing data for K-Means clustering. The transition from 4 clusters in the original dataset to 3 clusters in the PCA dataset illustrates how dimensionality reduction can alter the optimal configuration for data segmentation. Overall, using PCA can enhance the clustering process, leading to clearer insights into the relationships among cryptocurrencies while reducing the complexity of the analysis. Further research could involve exploring additional clustering algorithms and validating the results through external validation techniques to assess the robustness of the findings.
