# 🤝 K-Nearest Neighbors (KNN) Classification

## 📋 About K-Nearest Neighbors

K-Nearest Neighbors (KNN) is a simple yet powerful machine learning algorithm used for classification and regression tasks.  
It is a non-parametric, instance-based learning method that makes predictions by finding the most common label among the k closest training examples in the feature space.

The algorithm works based on distance metrics (like Euclidean distance) and does not make assumptions about the underlying data distribution.  
Because of its simplicity and effectiveness, KNN is widely used in many real-world applications, including medical diagnosis, recommendation systems, and anomaly detection.

I used the same dataset across my Decision Tree, KNN, and Random Forest models to ensure consistency and fair comparison.

---

## ⚙️ How KNN Works

- Find the k training samples closest in distance to the new point.
- Assign the most common label among those k neighbors to the new point.
- No learning happens during training; the model "learns" at the time of prediction.

---

## ✅ Advantages of KNN

- Simple and easy to implement.
- No need for model training (lazy learning).
- Naturally handles multi-class classification problems.

---

## ⚠️ Limitations of KNN

- Slow prediction time for large datasets.
- Sensitive to feature scaling and irrelevant features.
- Requires careful selection of the number of neighbors (k).

---

# 🩺 Breast Cancer Classification with KNN

## 📝 Project Description

In this project, I used the K-Nearest Neighbors (KNN) algorithm to classify breast cancer tumors into malignant or benign categories.  
The dataset used is the Breast Cancer Wisconsin dataset, which contains real-world medical diagnostic data.

Instead of using a complex model, I focused on observing how well a simple KNN model could perform on a realistic, high-dimensional medical dataset.

---

## 🗂️ Dataset Information

- **Name:** Breast Cancer Wisconsin (Diagnostic)
- **Samples:** 569
- **Features:** 30 numeric features related to tumor properties (radius, texture, perimeter, etc.)
- **Target Classes:**
  - 0 = Malignant
  - 1 = Benign

---

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---

## 🛠️ Installation

1. Clone the repository.
2. Install the required libraries:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn


# Project Workflow

## Step 1: Import Libraries and Load Data

- Imported libraries for data manipulation, visualization, and modeling.
- Loaded the Breast Cancer dataset from scikit-learn.

## Step 2: Preprocessing (Scaling and Train-Test Split)

- Standardized features using StandardScaler.
- Split the dataset into training and test sets with stratified sampling (80% train, 20% test).

## Step 3: Data Visualization (Class Distribution)

- Created a countplot to visualize the distribution of malignant and benign cases.

## Step 4: PCA Scatter Plot

- Applied PCA to reduce dimensionality to 2 components.
- Plotted the first two principal components to visualize class separation between benign and malignant tumors.

## Step 5: Build and Train KNN Model

- Initialized the KNN model with k=5 neighbors.
- Trained the model on the scaled training data.

## Step 6: Model Evaluation

- Predicted test labels and calculated test accuracy (~96.49%).
- Plotted a confusion matrix to evaluate true positives, true negatives, false positives, and false negatives.
- Generated a classification report to summarize precision, recall, and F1-score.

## Step 7: Accuracy vs Number of Neighbors (k)

- Explored different values of k (from 1 to 20).
- Plotted accuracy against the number of neighbors to find the optimal value of k.

## Step 8: Error Rate vs Number of Neighbors (k)

- Plotted error rate (1 - accuracy) against the number of neighbors.
- Provided an alternative view to better understand model behavior.

# Model Architecture

- Algorithm: K-Nearest Neighbors (KNN)
- Distance Metric: Euclidean Distance
- Initial number of neighbors: 5 (then explored 1-20)

# Results

- Test Accuracy: 96.49%
- Precision:
  - 0.97 for malignant
  - 0.96 for benign
- Recall:
  - 0.93 for malignant
  - 0.99 for benign
- F1-Score:
  - 0.95 for malignant
  - 0.97 for benign

The KNN model demonstrated high accuracy and strong generalization to unseen data.

# Visualizations

- Class Distribution Plot
- PCA Scatter Plot
- Confusion Matrix
- Classification Report
- Accuracy vs k Plot
- Error Rate vs k Plot

# Limitations

- KNN is sensitive to the choice of distance metric and scaling of features.
- Prediction time increases significantly with larger datasets.
- Feature selection could further improve model performance.

# Future Improvements

- Perform cross-validation to better tune k values.
- Test different distance metrics (e.g., Manhattan, Minkowski).
- Apply feature selection or dimensionality reduction.
- Compare KNN performance against Logistic Regression, SVM, or Decision Trees.

# Conclusion

Using K-Nearest Neighbors for classifying breast cancer tumors yielded excellent results with a test accuracy of around 96%.  
Through feature scaling, careful model evaluation, and tuning k values, I was able to optimize performance.  
While KNN is not always the best for larger datasets, it was very effective for this medical classification task.

# Author

- Beyza İspir

