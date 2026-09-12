# SmartCart Customer Segmentation

## Project Overview

SmartCart Customer Segmentation is an **Unsupervised Learning** project that uses customer data to identify different groups of
customers based on their characteristics and purchasing behavior.

The project applies **PCA K-Means Clustering, and Agglomerative Clustering** to discover meaningful customer segments.

## Objective

The main objectives of this project are:
- Clean and preprocess customer data
- Perform feature engineering
- Handle outliers and categorical features
- Reduce dimensionality using PCA
- Determine a suitable number of clusters
- Perform customer segmentation using clustering algorithms
- Analyze and interpret the resulting customer groups

## Dataset

The dataset contains **2,240 customer records** with information related to:

- Customer income
- Age
- Recency
- Purchasing behavior
- Website, catalog, and store purchases
- Campaign response
- Number of children
- Education
- Living arrangement
- Total spending

## Technologies & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- KneeLocator

## Project Workflow

The project follows these major steps:

1. Load the dataset
2. Explore the data
3. Handle missing values
4. Perform feature engineering
5. Remove outliers 
6. Analyse correlations
7. Encode categorical features
8. Scale the features
9. Apply PCA for dimensionality reduction
10. Use the Elbow Method and Silhouette Score to evaluate the number of clusters
11. Apply K-Means Clustering
12. Apply Agglomertive Clustering
13. Analyse and interpret customer segments

## Dimensionality Reduction

PCA was applied after feature scaling to reduce the dimensionality of the dataset.

Three principal components were used for visualisation and clustering analysis.

## Clustering

Different values of K were evaluated using:
- WCSS/Elbow Method
- Silhouette Score

The Elbow Method indicated **K =4** as a suitable choice.

Although some higher K values produced slightly higher Silhouette Scores, K=4, was selected because the resulting customer segments
were easier to interpret and provided meaningful business insights.

## Customer Segments

Four customer segments were indentified:

### Cluster 0- Low Spending Customers

- Lower average income
- Low total spending
- More Children on average
- Mostly living with a partner

### Cluster 1- High Value Customers

- Higher average income
- Very low total spending
- Mostly living alone
- Lower purchasing activity

### Cluster 2- Low Income/ Low Spending Customers

- Lower average income
- Very low total spending
- Mostly living alone
- Lower purchasing activity

### Cluster 3- High Value & Responsive Customers

- Higher average income
- High total spending
- Mostly living alone Higher campaign response
