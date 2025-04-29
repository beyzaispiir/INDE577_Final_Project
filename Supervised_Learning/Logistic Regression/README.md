# 🧠 Logistic Regression from Scratch

In this project, I built a Logistic Regression model from scratch to classify customer behavior. I manually handled data generation, weight updates, loss calculation, and model evaluation without using high-level libraries like `sklearn` for the modeling part. 

The focus was to understand the internal workings of Logistic Regression — including gradient descent optimization and the decision boundary formation.

---

## 📚 Algorithms Implemented

- **Logistic Regression** using:
  - Manual implementation of gradient descent.
  - Sigmoid activation for probability prediction.
  - Cross-entropy loss calculation.
  - Model evaluation using accuracy and cross-validation.
- **Visualization**:
  - Feature scatter plot.
  - Decision boundary visualization.
  - Training loss curve over epochs.
- **Cross-Validation**:
  - 5-Fold Cross-Validation to evaluate generalization performance.

---

## 🗂 Dataset Summary

- **Dataset Type**: Synthetic, generated within the notebook.
- **Features**: Two numerical features (`X1` and `X2`).
- **Target**: A binary label (Class 0 or Class 1) based on a threshold applied to a continuous combination of `X1` and `X2`.
- **Classes**: 
  - **Class 0**: Customers with lower combined scores.
  - **Class 1**: Customers with higher combined scores.

*This synthetic dataset was created to simulate a classification problem where `X1` strongly influences the target class.*

---

## 🛠 Instructions to Reproduce Results

1. Clone this repository or download the project files.
2. Make sure you have the required libraries installed:
    ```bash
    pip install numpy matplotlib seaborn
    ```
3. Run the Jupyter Notebook file (`logistic_regression_from_scratch.ipynb`) step-by-step:
    - **Step 1**: Generate and visualize the dataset.
    - **Step 2**: Build the custom Logistic Regression class.
    - **Step 3**: Train the model on the synthetic data.
    - **Step 4**: Visualize the learned decision boundary.
    - **Step 5**: Plot the training loss curve.
    - **Step 6**: Perform 5-Fold Cross-Validation to evaluate model performance.

4. Review outputs:
    - Scatter plots, decision boundary plots, and loss curve.
    - Accuracy results on training and validation splits.

---

## 📈 Key Results

- **Training Accuracy**: ~91.5%
- **Cross-Validation Accuracy**: ~89.0%
- **Loss Curve**: Smooth convergence without instability.
- **Decision Boundary**: Cleanly separates the two classes.

---

## 🎯 Key Takeaways

- Logistic Regression works well for simple binary classification tasks.
- A linear boundary is sufficient when features are well-separated.
- Understanding the optimization of the loss function deepens the intuition behind machine learning models.

---

## 📌 Notes

- I implemented the model **manually without using sklearn's LogisticRegression** to better understand the math and mechanics behind the algorithm.
- Some randomness in data generation may slightly vary results each time the notebook is run.

---

