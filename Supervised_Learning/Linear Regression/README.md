# 🏡 Linear Regression on California Housing Data

This project implements a **custom Linear Regression model** from scratch to predict the **median house value** based on selected features from the California Housing dataset.
Alongside building the model manually, I also compared its performance against Scikit-Learn’s `LinearRegression`, applied feature scaling, performed cross-validation, and analyzed residuals to evaluate model performance.

---

## 📚 Algorithms Implemented

- **Custom Linear Regression (Ordinary Least Squares)**:  
  Manually computed coefficients, intercept, standard errors, t-statistics, and p-values.
  
- **Feature Standardization**:  
  Standardized features using **StandardScaler** to improve numerical stability.
  
- **Cross-Validation (5-Fold)**:  
  Evaluated model generalization by averaging R² scores across 5 folds.

- **Residual Analysis**:  
  Analyzed model errors with residual plots and distribution graphs to check assumptions (e.g., homoscedasticity, normality).

---

## 📈 Dataset Summary

- **Dataset Used:**  
  [California Housing Prices Dataset (housing.csv)](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

- **Features Selected:**  
  - `median_income`
  - `housing_median_age`
  - `total_rooms`

- **Target Variable:**  
  - `median_house_value`

- **Preprocessing Steps:**  
  - Filled missing values in `total_bedrooms` using the column median.
  - Selected a subset of features for modeling.
  - Standardized features during advanced training.

---

## ⚙️ Instructions for Reproducing the Results

1. **Clone the repository or download the files.**

2. **Install required libraries:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```

3. **Place `housing.csv` in the same directory as the notebook.**

4. **Run the notebook cells step-by-step:**
   - Import libraries
   - Load and clean the data
   - Explore features vs. target
   - Train and evaluate the custom Linear Regression model
   - Compare results with Scikit-Learn
   - Apply feature scaling and retrain
   - Perform 5-Fold Cross-Validation
   - Analyze residuals and error distribution

---

## 📌 Key Takeaways

- Median income was the strongest predictor of median house value.
- Scaling improved stability but model performance stayed roughly similar.
- Residual plots revealed patterns suggesting a simple linear model may not be sufficient for all patterns in the data.
- Building a regression model from scratch greatly improved understanding of how coefficients, statistical tests, and model diagnostics are performed internally.

---

