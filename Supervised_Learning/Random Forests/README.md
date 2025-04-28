# 🌳 Random Forest Classifier on Breast Cancer Dataset

## 📋 Introduction

This project implements a Random Forest Classifier to predict whether a tumor is malignant or benign based on the Breast Cancer dataset from Scikit-learn.  
Random Forest is an ensemble learning technique that combines multiple decision trees to improve prediction accuracy and reduce overfitting.  
I used the same dataset across my Decision Tree, Neural Network, and Random Forest models to ensure consistency and fair comparison.

---

## 📚 Algorithms Implemented

- Random Forest Classifier
- Hyperparameter Tuning with GridSearchCV
- Feature Importance Analysis
- Error Analysis based on Residuals
- Accuracy vs Number of Estimators Analysis

---

## 🗂️ Dataset Information

- **Dataset:** Breast Cancer Wisconsin Dataset
- **Source:** `sklearn.datasets.load_breast_cancer`
- **Number of samples:** 569
- **Number of features:** 30 numerical features
- **Classes:** 
  - 0 = Malignant
  - 1 = Benign

**Selected Features:**
- mean radius
- mean texture
- mean perimeter
- mean area
- mean smoothness
- ... *(and more - total 30 features)*

---

## 📦 Packages Used

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `joblib`

---

## 🛠️ How to Reproduce

1. **Clone the repository** or download the notebook files.
2. **Install the required packages:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn joblib

