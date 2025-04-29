# DBSCAN Clustering on Mall Customer Segmentation Dataset

## 🧠 Introduction

In this project, I applied the DBSCAN clustering algorithm to the Mall Customer Segmentation dataset.  
The goal was to discover natural groupings of customers based on their annual income and spending score, without any supervision.  
DBSCAN is a powerful clustering technique because it can find clusters of varying shapes and detect outliers (noise points) without needing to predefine the number of clusters.

---

## 🛠 Project Steps

- Loaded the Mall Customers dataset.
- Explored the data and visualized feature distributions.
- Selected the two most relevant features: **Annual Income (k$)** and **Spending Score (1-100)**.
- Standardized the selected features to make them comparable.
- Applied **DBSCAN** to find clusters in the customer data.
- Visualized the clusters using 2D scatter plots.
- Highlighted the noise points detected by DBSCAN.
- Evaluated the clustering performance using **Silhouette Score**.

---

## 📚 Dataset Summary

- **Name:** Mall Customers Dataset
- **Samples:** 200 customers
- **Features Used:** Annual Income (k$), Spending Score (1-100)
- **Target:** No explicit target; unsupervised clustering task.

---

## ⚙️ How to Reproduce

1. Clone or download this repository.
2. Install the required Python libraries if you don't have them yet:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
## ⚙️ How to Reproduce

Run the notebook in **Jupyter Notebook** or your preferred Python environment.

Steps covered inside the notebook:

- Import libraries and load the dataset.
- Check for missing values and explore feature distributions.
- Standardize features using `StandardScaler`.
- Apply **DBSCAN** with chosen `eps` and `min_samples` parameters.
- Visualize clustering results and noise points.
- Calculate the **Silhouette Score**.

---

## 📈 Visual Outputs Included

- **Pairplot of Selected Features:**  
  Visualized the distribution of annual income and spending score to understand feature scales and relationships before clustering.

- **DBSCAN Cluster Visualization (Standardized Features):**  
  Showed customer groups detected by DBSCAN in a 2D scatter plot.  
  Each color represented a different cluster, and noise points were automatically separated.

- **DBSCAN Noise Points Highlighted:**  
  A separate plot specifically highlighting noise points (outliers) in **red**, and regular cluster members in **blue**.

- **Estimated Number of Clusters and Silhouette Score:**  
  Printed outputs showing:
  - Total number of clusters (excluding noise).
  - Number of noise points.
  - Silhouette Score to evaluate clustering quality (higher is better).

---

## 🎯 Key Learning Points

- DBSCAN can identify clusters of different shapes and automatically detect noise points.
- Standardizing features is essential before applying DBSCAN because the algorithm is sensitive to distances.
- Visualizations like scatter plots and noise point highlighting help to better interpret the clustering results.
- The Silhouette Score provides a useful metric to evaluate how well the clustering separated the data.
- Tuning `eps` (maximum distance between two samples) and `min_samples` (minimum number of points to form a cluster) is crucial for achieving meaningful results.

