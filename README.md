🧩 Customer Segmentation Using K-Means Clustering
📘 Overview

This project performs customer segmentation using K-Means clustering. It identifies distinct groups of customers based on purchasing behavior and demographic data, helping businesses tailor their marketing strategies, improve customer targeting, and increase overall satisfaction.

The notebook automates the entire workflow — from data loading to visualization and interpretation of clusters.

🧠 Key Features

Data loading from CSV (unprocessed_customer_data_tamilnadu.csv)

Data cleaning and preprocessing (handling missing values, scaling)

Feature engineering (e.g., Average Purchase Value)

Correlation analysis and visualization

Dimensionality reduction using PCA (Principal Component Analysis)

Optimal cluster selection using Elbow Method

Clustering with K-Means Algorithm

Visualization of clusters in 2D PCA space

Cluster-wise summary statistics

⚙️ Workflow Summary
1. Data Import & Setup

Mounted Google Drive for data access.

Loaded dataset using pandas.

Displayed initial records for inspection.

2. Data Preprocessing

Checked for null values.

Filled missing numeric data using column means.

Derived new metrics (e.g., AvgPurchaseValue = TotalSpent / TotalVisits).

3. Exploratory Data Analysis (EDA)

Generated summary statistics with describe().

Visualized correlation heatmap using Seaborn.

Plotted distribution of key numerical features.

4. Feature Scaling

Applied StandardScaler from sklearn.preprocessing to normalize data for clustering.

5. Finding Optimal Number of Clusters

Used Elbow Method with KElbowVisualizer from yellowbrick.cluster.

Determined the best k value for clustering.

6. Model Training & Clustering

Applied K-Means algorithm with the optimal cluster count.

Assigned cluster labels to each record in the DataFrame.

7. Dimensionality Reduction & Visualization

Reduced data to 2D using PCA.

Visualized clusters using Seaborn scatterplots.

8. Cluster Analysis

Computed mean feature values for each cluster.

Interpreted customer groups based on behavioral and spending attributes.

🧩 Technologies Used
Category	Libraries
Data Handling	pandas, numpy
Visualization	matplotlib, seaborn, yellowbrick
Machine Learning	scikit-learn
Dimensionality Reduction	PCA (from sklearn.decomposition)
Environment	Google Colab
📈 Outputs

Heatmap showing correlations between features

Elbow plot for optimal K selection

PCA-based cluster visualization

Cluster summary table showing key differentiating metrics

🚀 How to Run

Upload the notebook to Google Colab.

Mount your Google Drive:

from google.colab import drive
drive.mount('/content/drive')


Place your dataset (unprocessed_customer_data_tamilnadu.csv) in your Drive.

Update the file path in the notebook if necessary.

Run all cells sequentially.
