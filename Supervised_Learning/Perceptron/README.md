# 🧠 Perceptron Learning from Scratch

In this project, I implemented a Perceptron model from scratch to predict customer purchase behavior based on two features: **Annual Income** and **Spending Score**.  
The project covers basic supervised learning concepts, manual dataset creation, visualization of feature relationships, training a Perceptron classifier, and evaluating its performance through learning curves and decision boundaries.

---

## 📚 Algorithm Implemented

- **Perceptron Classifier**:
  - Manually implemented weight updates, prediction functions, and training loops.
  - Used a basic learning rule with gradient descent to minimize classification errors.
  - Visualizations include decision boundary plots and learning curves.

---

## 📊 Dataset Summary

- **Data Source**:  
  Synthetic dataset manually created for demonstration purposes.
  
- **Features**:
  - Age
  - Annual Income (k$)
  - Spending Score (1-100)

- **Target**:
  - Purchase (0 = No, 1 = Yes)

- **Highlights**:
  - Spending behavior is a stronger predictor than income.
  - Income alone does not reliably separate classes.

---

## 🚀 Instructions to Reproduce

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/perceptron-learning.git
   cd perceptron-learning
   ```

2. **Install Dependencies**:
   ```bash
   pip install numpy pandas matplotlib seaborn
   ```

3. **Run the Notebook**:
   Open `Perceptron_Learning.ipynb` and execute all cells to reproduce the results.

---

## 📈 Key Results

- **Decision Boundary**:  
  The Perceptron model learned a linear boundary separating purchase decisions based on spending and income.

- **Learning Curve**:  
  The number of misclassifications stabilized but did not reach zero, highlighting the model's limitations on imperfectly separable data.

---

## 📝 Project Structure

```
├── Perceptron_Learning.ipynb   # Main Jupyter notebook
├── README.md                   # Project documentation
```

---

## ✨ Final Notes

- The Perceptron model works well for linearly separable datasets.
- Non-linear boundaries require more complex models like logistic regression or neural networks.
- This project helped me deeply understand supervised learning concepts, model training mechanics, and error analysis.


