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

