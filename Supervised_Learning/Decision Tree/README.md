# 🌳 Decision Trees on Breast Cancer Dataset

## 📋 About Decision Trees

Decision Trees are a simple yet powerful supervised machine learning algorithm used for both classification and regression tasks.  
The idea is to model decisions and their possible consequences as a tree structure, with internal nodes representing decision points based on feature values and leaf nodes representing predicted outcomes.

I chose Decision Trees because they provide easy interpretability, allow visualization of the decision-making process, and do not require feature scaling or normalization.

In classification problems like this, the algorithm splits the data into subsets based on the most informative features, using criteria like **Gini Index** or **Entropy (Information Gain)** to choose the best splits.  
Although Decision Trees are prone to overfitting, controlling the maximum depth and pruning techniques can significantly improve their generalization.

I used the same dataset across my Decision Tree, KNN, and Random Forest models to ensure consistency and fair comparison.


---

## 🗂️ Summary of the Dataset

For this project, I used the **Breast Cancer Wisconsin** dataset, which is a standard dataset included in Scikit-learn.

- **Samples:** 569
- **Features:** 30 numerical features (e.g., radius, texture, smoothness, etc.)
- **Target Classes:**
  - 0 = Malignant (cancerous)
  - 1 = Benign (non-cancerous)

The dataset is moderately imbalanced with more benign samples than malignant ones, which I took into account during model evaluation.

---

## 🔄 Key Steps and Visualizations

### 📌 1. Load and Explore Data

- Loaded the data, checked the shapes, and visualized the class distribution.
- Initial exploration showed that benign tumors are slightly more common.

### 📌 2. Train-Test Split

- Split the data into 80% training and 20% testing sets.
- Ensured stratification to preserve class balance between malignant and benign cases.

### 📌 3. Model Training

- Trained two types of Decision Trees:
  - A **full tree** without depth limitation (to observe overfitting).
  - A **pruned tree** with **max_depth=4** to improve generalization.

### 📌 4. Evaluation

- Evaluated models using:
  - Test Accuracy
  - Confusion Matrix
  - Precision, Recall, F1-score
  - Visualization of the tree structure

- The limited-depth tree achieved better balance between bias and variance, with a **Test Accuracy of 93.86%**.

### 📌 5. Feature Importance

- Plotted feature importances assigned by the Decision Tree.
- Features like **worst radius** and **worst concave points** were identified as the most critical factors for prediction.

### 📌 6. Training vs Testing Accuracy vs Tree Depth

- Created a plot showing how accuracy evolves with tree depth.
- Confirmed that allowing unrestricted depth leads to perfect training accuracy (overfitting), while a depth of around 4-5 gives the best testing performance.

---

## 🛠️ How to Reproduce My Results

Follow these steps to reproduce the project:

1. **Install required packages** (if not already installed):
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn

2. **Clone the repository** or simply copy the files into your working directory.

3. **Run the Jupyter Notebook or Python script** containing:
    - Data loading
    - Train-test split
    - Decision Tree training
    - Evaluation (confusion matrix, accuracy, feature importance, tree visualization)

4. **(Optional)** Adjust `max_depth` parameter to observe how overfitting/underfitting behaviors change.

---

## Important Notes About Decision Trees

- Decision Trees do **not require feature scaling** (no need for StandardScaler).
- Trees can perfectly memorize training data if not pruned, but this hurts test performance.
- Setting a maximum depth or using pruning helps prevent overfitting.
- Feature importance scores give great insights into what drives the classification decisions.
- Entropy and Gini index are the two most common splitting criteria:
  - **Gini** favors pure splits.
  - **Entropy** is based on information theory and measures uncertainty.

---

## References
This project was inspired by decision tree theory, including concepts like:
- Entropy
- Gini Index
- Pre-pruning and Post-pruning

Additional theoretical background can be found [here](https://en.wikipedia.org/wiki/Decision_tree_learning).

---

