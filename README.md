# Human-Activity-Recognition-SmartActivityClustering
A machine learning project using clustering algorithms to group human activity data from smartphones. This project leverages accelerometer and gyroscope data from the "Human Activity Recognition Using Smartphones" dataset, applying unsupervised learning techniques for activity classification.

# SmartActivityClustering

## Project Overview
This project focuses on clustering human activity data using unsupervised learning algorithms. The dataset used is the "Human Activity Recognition Using Smartphones" dataset from the UCI Machine Learning Repository. The dataset includes sensor data from accelerometers and gyroscopes embedded in smartphones carried by 30 participants, performing six different activities: walking, walking upstairs, walking downstairs, sitting, standing, and laying.

The goal of the project is to apply various clustering algorithms to group similar activities together based on the sensor data.

## Dataset
The dataset contains 561 features, which include time-domain and frequency-domain variables derived from the accelerometers and gyroscopes. The activities performed are:

- Walking
- Walking upstairs
- Walking downstairs
- Sitting
- Standing
- Laying

The dataset is pre-processed and transformed for easy use in machine learning models.

## Objectives
1. To cluster the human activity data into distinct groups representing different activities.
2. To experiment with different clustering algorithms (e.g., K-Means, Hierarchical Clustering, DBSCAN) and evaluate their effectiveness in distinguishing between different activities.
3. To visualize the clusters using appropriate dimensionality reduction techniques such as PCA or t-SNE.

## Technologies Used
- **Programming Language**: Python
- **Libraries**:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
- **Development Environment**: Google Colab

 
Here I have chosen three main clustering methods. 
1. K-Means Clustering Method 
2. Hierarchical Clustering 
3.  DBSCAN 
 
 K- Means Clustering Method: 
K-Means is a centroid-based clustering algorithm that partitions data into K 
clusters. The algorithm assigns each data point to the nearest cluster center and 
then updates the cluster centers as the mean of the assigned points. This process 
is iterated until the cluster assignments no longer change. 
 
• Why Chosen: 
Efficiency: K-Means is computationally efficient and works well for large datasets. 
Simplicity: It is easy to understand and implement. 
Scalability: Handles large datasets and high-dimensional spaces effectively. 
 
 
• Considerations: 
The number of clusters K must be specified beforehand. 
Sensitive to the initial placement of cluster centers and outliers. 
 
Hierarchical Clustering: 
Hierarchical clustering builds a tree of clusters (dendrogram) either by 
successively merging smaller clusters (agglomerative approach) or by successively 
splitting larger clusters (divisive approach). The algorithm does not require 
specifying the number of clusters in advance. 
 
• Why Chosen: 
No Need for Pre-Specified K: You can determine the number of clusters by cutting 
the dendrogram at the desired level. 
Flexibility: Provides a hierarchy of clusters, allowing for different cluster 
granularities. 
Interpretability: The dendrogram helps in understanding the clustering structure. 
 
• Considerations: 
Computationally expensive for large datasets. 
Choice of distance metric and linkage criteria can affect results. 
 
 

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) 
DBSCAN is a density-based clustering algorithm that groups together points that 
are close to each other based on a distance metric and a minimum number of 
points. It can identify clusters of arbitrary shape and handle noise (outliers) 
effectively. 
 
• Why Chosen: 
Detects Arbitrary Shapes: Can find clusters with non-spherical shapes that K
Means might miss. 
Handles Noise: Identifies outliers as noise, which is useful in real-world data with 
potential outliers. 
No Need for K: Does not require specifying the number of clusters in advance. 
 
• Considerations: 
Requires setting parameters like 'eps' (distance threshold) and 'min_samples' 
(minimum number of points). 
Performance can vary depending on parameter settings and dataset density.

 Improvisation of the overall experiment. 
 
Adjusting key parameters for the clustering algorithms, such as the ‘eps’ 
and ‘min_samples’ in DBSCAN, helped in identifying more meaningful 
clusters. This tuning ensures that the algorithms better capture the true 
structure of the data, reducing noise and improving cluster separation. 
 
By refining these parameters, DBSCAN can more effectively distinguish 
between noise (outliers) and meaningful clusters, leading to cleaner and 
more accurate results.

 
Based on the above evaluation metrics, K-Means clustering is recommended for 
this dataset due to its superior performance across various metrics. However, if 
outlier detection is a priority, DBSCAN can be considered with tuned parameters.  
 
 
Precautions took to avoid overfitting and underfitting: 
 
1. Overfitting: 
 
• Feature Scaling:  
         Normalized the dataset using ‘StandardScaler’ to verify that each 
feature contributes equally to the model. 
 
• Evaluating Clustering Using Several Metrics: 
         Several metrics (Silhouette Score, Davies-Bouldin Index, and 
Calinski-Harabasz Index) were used to evaluate the clustering findings in 
order to make sure the clusters were relevant and did not overfit the 
data. 
 
• Outlier Detection: 
        K-Means, DBSCAN, and hierarchical clustering algorithms were used 
to identify outliers in order to determine whether any particular data 
points were unfairly influencing the clustering findings. 
2. Underfitting: 
 
• Selecting a Range of Indicators: 
        To make sure the models are highly accurate to represent the 
underlying structure in the data, a variety of clusters (k for K-Means and 
eps values for DBSCAN) were investigated. 
 
• Visual Inspection: 
        To make sure the clusters make sense and that the clustering model 
captures significant patterns in the data, the clustering results were 
visualized and carefully examined. 
 
• Adjusting Parameters Based on Evaluation: 
       The parameters were used to adjust hyperparameters in DBSCAN, 
such as the number of clusters and eps value, to make sure the models 
are neither either complicated (overfitting) nor too simple (underfitting).
