Customer Segmentation with K-Means & PCA

This project applies unsupervised learning to identify distinct customer segments based on their purchasing behavior. Using K-Means clustering and Principal Component Analysis (PCA), we can visualize and interpret the different customer groups, enabling better marketing and business strategies.

Project Overview

  Objective: Discover distinct customer groups to enable targeted marketing strategies.
  Core Techniques: K-Means Clustering, Elbow Method, Standardization, PCA Visualization.
  Dataset: Mall Customers Dataset from Kaggle.
  Outcome: Segmented customers into 5 groups based on their Annual Income and Spending Score.


Workflow

  Load & Explore Data: Understand the structure and key features of the dataset.
  Preprocess Data: Select relevant features and apply scaling (critical for K-Means).
  Determine Optimal Number of Clusters using the Elbow Method.
  Apply K-Means Clustering to group customers.
  Visualize Clusters using scatter plots and PCA.
  Interpret Segments: Turn clusters into actionable business insights.

Project Structure

customer-segmentation/
│
├── Mall_Customers.csv             # Dataset from Kaggle
├── customer_segmentation.py       # Main Python script
└── README.md                      # Project documentation

Requirements
Install dependencies via pip:pip install pandas numpy scikit-learn matplotlib seaborn

Key Features Used

Annual Income (k$)
Spending Score (1–100)
(Other features like Age can be used for further analysis of segments.)

Exploratory Analysis

Elbow Method Plot: Shows Within-Cluster-Sum-of-Squares (WCSS) vs. k to find optimal clusters.
Scatter Plot of Clusters: Visualizes customer segments by income and spending score.
Centroids: Red markers showing the center of each cluster.

Segments Identified
Segment	Characteristics	Business Insight
0 – Standard	Average income, average spending	Baseline customers
1 – Target (Prime Customers)	High income, high spending	High-value customers to retain
2 – Careful	High income, low spending	Upsell or retarget campaigns
3 – Sensible	Low income, low spending	Low-value customers
4 – Careless	Low income, high spending	Budget-friendly offers

(Segment personas can be refined further by combining Age and other demographic data.)

Future Improvements

Include Age, Gender, or other demographics for more nuanced segmentation.
Use PCA to reduce dimensionality when using multiple features.
Experiment with other clustering methods (DBSCAN, Hierarchical Clustering).

Output

Cluster Labels added to the original dataset.
Visualizations of clusters and centroids.
Segment Analysis Table showing average Age, Income, and Spending Score for each group.

License
This project is for educational purposes and based on publicly available datasets from Kaggle.


  
