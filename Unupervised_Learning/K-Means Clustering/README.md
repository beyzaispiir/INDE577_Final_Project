# 🍷 K-Means Clustering on Red Wine Quality Dataset

## 📚 About K-Means Clustering

K-Means Clustering is one of the most popular unsupervised learning algorithms used to find groups (clusters) in data.  
It works by partitioning the dataset into k distinct clusters based on feature similarity.  
Each data point is assigned to the nearest cluster center (called centroid), and the centroids are updated iteratively to minimize the distance between the points and their assigned centers.

K-Means assumes that:
- Clusters are roughly spherical and similar in size.
- Features are continuous and comparable.

Although K-Means is simple, it is very powerful and widely used in real-world tasks like:
- Customer segmentation
- Market basket analysis
- Image compression
- Document clustering

In this project, I used K-Means to explore hidden structures among different types of red wines based on their chemical properties.

---

## 📂 Project Description

In this project, I:
- Loaded and preprocessed the Red Wine Quality dataset.
- Used two features (**Density** and **Alcohol**) for initial visualization and clustering.
- Applied the **Elbow Method** and **Silhouette Score** to find the best number of clusters.
- Expanded clustering by adding a third feature (**pH**) and visualized the results in 3D.
- Analyzed how wines naturally grouped without using their quality labels.

This helped me understand how clustering can reveal meaningful patterns even without any supervision.

---

## 🛠 Dataset Summary

- **Name:** Red Wine Quality Dataset
- **Source:** UCI Machine Learning Repository
- **Samples:** 1,599 red wine samples
- **Features:** 12 physicochemical properties (like acidity, sugar, sulfur dioxide, alcohol, etc.)
- **Target:** Wine quality scores (not used for training, only for reference)

Dataset link:
https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv

## ⚙️ How to Reproduce This Project

To reproduce my results, follow these steps:

1. **Clone** this repository to your local machine.
2. **Install** the required libraries if they are not already installed:
   ```bash
   pip install numpy pandas matplotlib scikit-learn

## ▶️ Running the Notebook

After installing the requirements, you can run the notebook in **Jupyter Notebook** or any other Python environment.

The notebook covers the following steps:
- Import libraries and load the dataset.
- Explore and preprocess the data.
- Use the Elbow Method and Silhouette Analysis to find the optimal number of clusters (K).
- Train K-Means models and visualize clusters in 2D and 3D.

---

## 📈 Visual Outputs Included

- Scatter plots of wine samples by alcohol and density
- Elbow curve to determine the optimal number of clusters
- Silhouette score plots for cluster quality analysis
- 2D and 3D visualizations of clustering results
- Cluster size bar charts

---

## 🎯 Key Learning Points

- K-Means works well for discovering natural groupings even without any labeled data.
- Choosing the right number of clusters (K) is critical for better interpretation.
- Adding more features (like pH) can enhance cluster separation but requires careful visualization.
- Silhouette Score is a useful additional check beyond the Elbow Method.
