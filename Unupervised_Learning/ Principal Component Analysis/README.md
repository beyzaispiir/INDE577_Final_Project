# 🍷 Principal Component Analysis (PCA) on Red Wine Quality Dataset

## 📚 About PCA Algorithm

Principal Component Analysis (PCA) is a powerful unsupervised learning method used mainly for dimensionality reduction.  
It transforms the original set of features into a smaller set of new features, called principal components, while preserving as much of the data’s variation as possible.  

Each principal component captures the direction of maximum variance in the data, with the first component carrying the most information, the second component carrying the next most, and so on.  
PCA helps to simplify complex datasets, reveal hidden structures, reduce noise, and improve visualization — especially in high-dimensional datasets.  

In real-world applications, PCA is commonly used for:
- Data visualization (2D or 3D plots)
- Preprocessing before machine learning models
- Noise reduction
- Feature extraction and interpretation

In this project, I used PCA to explore and visualize how different chemical properties of red wines are related, without using wine quality labels during the dimensionality reduction process.

---

## 📂 Project Description

In this notebook, I:
- Loaded and prepared the Red Wine Quality dataset.
- Standardized all chemical features to have zero mean and unit variance.
- Applied PCA and calculated the explained variance for each principal component.
- Plotted a scree plot to observe how many components are useful.
- Projected the data onto the first two and three principal components.
- Created 2D and 3D visualizations colored by wine quality.
- Investigated the principal component loadings to understand which features contribute the most.

This approach allowed me to see the relationships among wines and their features without relying directly on labeled information.

---

## 🛠 Dataset Summary

- **Name:** Red Wine Quality Dataset
- **Source:** UCI Machine Learning Repository
- **Link:** [UCI Red Wine Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv)
- **Samples:** 1,599 wines
- **Features:** 11 physicochemical properties (like acidity, residual sugar, chlorides, alcohol, pH, etc.)
- **Target:** Wine quality score (integer between 3 and 8, but **not used** during PCA)

---

---

## 📚 Steps Covered Inside the Notebook

- Import libraries and load the Red Wine Quality dataset.
- Explore and preprocess the data.
- Standardize the features to ensure they are on the same scale.
- Apply Principal Component Analysis (PCA) and examine the explained variance.
- Visualize the results using 2D and 3D scatter plots.
- Analyze the principal component loadings to understand feature contributions.

---

## 📈 Visual Outputs Included

- Scree Plot showing explained variance by each principal component.
- 2D scatter plot projection onto the first two principal components.
- 3D scatter plot projection onto the first three principal components.
- Colorbar visualization based on wine quality scores.
- Table showing how each original feature contributes to each principal component (PCA loadings).

---

## 🎯 Key Learning Points

- PCA is an effective way to reveal structures and patterns in high-dimensional datasets.
- Standardizing the data before applying PCA is critical because PCA is sensitive to feature scaling.
- The first few principal components can often explain a large portion of the total variance.
- Visualizing data using principal components makes it easier to interpret and explore complex relationships.
- Analyzing the loadings provides insights into which features drive the major variations in the data.
