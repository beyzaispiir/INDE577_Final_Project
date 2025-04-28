# 🚀 Ensemble Learning for Customer Churn Prediction

This project applies two popular ensemble learning techniques — **Gradient Boosting** and **AdaBoost** — to predict customer churn using the **Telco Customer Churn Dataset**.  
By comparing the performance of both algorithms, I aimed to understand which method generalizes better and handles churn prediction more effectively.

---

## 📚 About Ensemble Methods

**Gradient Boosting** and **AdaBoost** are ensemble learning techniques that combine the predictions of multiple simple models (usually decision trees) to create a stronger overall model.

- **Gradient Boosting** builds models sequentially, with each new model correcting the errors made by the previous ones. It minimizes a loss function using gradient descent.
- **AdaBoost** adjusts the weights of incorrectly classified examples, forcing the next model to focus more on difficult cases.

In real-world applications, these methods are widely used for:
- Credit risk prediction
- Customer churn analysis
- Fraud detection
- Product recommendation systems
- Medical diagnosis

Both methods are valued for their ability to create highly accurate models while handling complex patterns in data.

---

## 📈 Dataset Summary

**Dataset Name:** Telco Customer Churn Dataset  
**Source:** [IBM Sample Data](https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv)

**Dataset Description:**
- 7043 samples
- 21 features (both categorical and numerical)
- Target variable: **Churn** (whether a customer leaves or stays)

Key features include:
- Customer demographics (age, gender, senior citizen)
- Services subscribed (InternetService, PhoneService, StreamingTV)
- Account information (Contract type, MonthlyCharges, Tenure)

This dataset reflects typical customer retention challenges in industries like telecoms and subscription services.

---

## ⚙️ Instructions to Reproduce the Results

Follow these steps to run the notebook and reproduce the analysis:

1. **Clone this repository** or download the notebook file.

2. **Install the required Python libraries** if you don't already have them:
    ```bash
    pip install numpy pandas matplotlib seaborn scikit-learn
    ```

3. **Open the Jupyter Notebook**.

4. **Run the cells in order**:
   - Import libraries
   - Load and prepare the dataset
   - Train Gradient Boosting and AdaBoost models
   - Compare models using accuracy, confusion matrices, feature importance, and ROC curves

5. **(Optional)** You can tweak hyperparameters like learning rate or number of estimators to see how model performance changes!

---

## 📊 Key Visualizations

Throughout the notebook, I included:
- Training vs Testing Accuracy Barplots
- Confusion Matrices (side-by-side comparison)
- Feature Importance Graphs for both models
- ROC Curves for direct comparison
- Printed AUC Scores and Analysis Summaries

These plots help understand not just which model performs better, but also **why** and **how** they differ.

---

## 🔥 Final Takeaways

- **Gradient Boosting** performed slightly better than **AdaBoost** on this dataset, based on accuracy and AUC score.
- Both models showed good generalization without major overfitting.
- Ensemble methods are incredibly effective for complex prediction tasks like churn analysis where many factors interact.

---

## ✨ Author

**Beyza İspir**  
Master of Industrial Engineering | Rice University

---
