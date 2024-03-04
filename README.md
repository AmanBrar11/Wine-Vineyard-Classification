# Wine Origin Classification Project
### Problem and Data Overview

In this project, we explore a popular dataset on wine from the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine), also accessible via the sklearn dataset collection. The dataset comprises 13 measurements of different constituents found in wines, originating from three separate vineyards. Our goal is to use these attributes to classify the vineyard of origin for each wine, comparing the performance of unsupervised and supervised models. This analysis is crucial for enhancing wine authenticity and traceability, vital for protecting the integrity of renowned wine-producing regions and preventing fraud in the industry.

### Exploratory Data Analysis

The exploratory phase involved understanding the distribution of the wine's attributes through violin plots and identifying outliers. This initial analysis was crucial for ensuring the quality of the subsequent models. The data was then split into training and testing sets to prepare for model building.

### Principal Component Analysis (PCA)

Given the limited accuracy achieved with all 13 features in initial models, PCA was applied to reduce the feature space to 9 components, explaining approximately 95% of the variance. This dimensionality reduction was a pivotal step in improving model performance.

### Agglomerative Clustering Model

An unsupervised agglomerative clustering model was selected for its suitability to the dataset's identifiable clusters. After fine-tuning, the best model achieved an impressive 97.7% accuracy using the "average" linkage method and "manhattan" metric.

### K-Nearest Neighbors Model

The supervised counterpart, a K-Nearest Neighbors (KNN) model, was chosen for its simplicity and versatility. Despite its potential, the best accuracy obtained was 75.8%, highlighting the unsupervised model's superior performance in this context.

### Results Discussion and Conclusion

The unsupervised Agglomerative Clustering model outperformed the supervised KNN model, suggesting that the wine attributes provided strong intrinsic clustering patterns. This study underscores the potential of machine learning in enhancing wine traceability and authenticity, opening avenues for integrating additional data sources in future work.

