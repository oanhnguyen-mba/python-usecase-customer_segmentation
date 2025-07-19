# Customer Segmentation with K-Means Clustering
This project demonstrates a customer segmentation use case using K-Means clustering on RFM (Recency, Frequency, Monetary) data. It is designed as an academic and business-oriented exercise to showcase how unsupervised learning techniques can support customer analytics and strategic decision-making in industries such as banking, e-commerce, and retail.

## Abstract
Customer segmentation is a critical step in understanding diverse customer behaviors and personalizing marketing strategies. By leveraging K-Means clustering on simulated RFM data, this project identifies distinct customer groups to enable targeted interventions. Principal Component Analysis (PCA) is used to visualize clusters in two dimensions. The results offer actionable insights for customer retention, reactivation, and value maximization.

## Methodology
### 1. Data Simulation:
A synthetic dataset of 200 customers was generated, including:
  - Recency (days since last purchase),
  - Frequency (number of purchases), and
  - Monetary (total spending).
### 2. Data Preprocessing:
Standardized RFM features using StandardScaler to remove scale bias.
### 3.Clustering:
Applied K-Means algorithm to segment customers into clusters.
Used the Elbow Method to determine the optimal number of clusters (k=3).
### 4. Dimensionality Reduction:
Applied PCA (Principal Component Analysis) to reduce RFM data from 3D to 2D for visualization.
### 5. Visualization:
Plotted cluster assignments using color-coded scatter plots.

## Requirements
Python >= 3.x

## Libraries:
pandas, numpy, matplotlib, seaborn, scikit-learn

## Results
### Cluster Summary
| Cluster | Recency (days) | Frequency | Monetary ($) | Insight                              |
|---------|----------------|-----------|--------------|------------------------------------|
| 0       | 272            | 35.7      | 719.8        | Lapsed VIPs: High spenders, inactive for long. |
| 1       | 83             | 34.6      | 470.9        | Current VIPs: Loyal, frequent, high spending.  |
| 2       | 223            | 15.9      | 199.8        | At Risk: Low frequency, low spending, inactive.|
| 3       | 156            | 8.1       | 753.8        | Big Spenders: Infrequent but large purchases.  |

### Key Visualizations
Elbow Method: Optimal clusters identified at k=3.
PCA Scatter Plot: Clear separation between customer segments.

## Managerial Implications
The clustering results provide actionable insights for customer management:
- Cluster 1 (Current VIPs): Prioritize for loyalty programs and exclusive offers to retain high-value customers.
- Cluster 0 (Lapsed VIPs): Implement win-back campaigns to reactivate valuable but inactive customers.
- Cluster 2 (At Risk): Focus on churn prevention strategies, such as personalized discounts or reminders.
- Cluster 3 (Big Spenders): Design strategies to increase purchase frequency, e.g., subscription models or VIP perks.
By understanding customer segments, businesses can allocate resources efficiently, maximize customer lifetime value, and drive growth.
