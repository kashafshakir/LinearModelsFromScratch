# 📊 Custom Linear, Ridge & Lasso Regression from Scratch (NumPy)

**Description:**  
This project demonstrates the implementation of **Linear, Ridge, and Lasso Regression from scratch** using **NumPy**, without relying on high-level libraries like `scikit-learn`.  
It is designed to illustrate a deep understanding of:

- Gradient Descent optimization  
- L1 and L2 regularization  
- Feature selection and coefficient shrinkage  
- Convergence visualization  

The project uses the **House Prices dataset (Kaggle)** as a case study to predict housing prices and visualize model behavior.

---

## 🚀 Features

- **Custom Linear Regression**
  - Implemented batch gradient descent
  - Tracked **Mean Squared Error (MSE)** across iterations
  - Visualization of **loss vs iterations** for convergence analysis

- **Custom Ridge Regression (L2)**
  - Implemented L2 regularization in gradient descent
  - Coefficient shrinkage visualization across different λ values
  - Comparison of Ridge vs Linear regression behavior

- **Custom Lasso Regression (L1)**
  - Implemented L1 regularization with gradient descent
  - Automatic feature selection (coefficients driven to zero)
  - Visualized **Lasso coefficient paths** across λ values

- **Feature Selection**
  - For Linear and Ridge Regression, feature selection was applied using **Random Forest feature importance**
  - Lasso inherently performs feature selection, so all features were retained

---

## 📊 Visualizations

1. **Loss vs Iterations** (Linear Regression)
   - Shows convergence of gradient descent

2. **Coefficient Paths vs Lambda** (Ridge & Lasso)
   - Ridge: Smooth shrinkage of coefficients  
   - Lasso: Some coefficients driven to zero (sparsity)

3. **Feature Sparsity vs Lambda** (Lasso)
   - Shows number of non-zero coefficients for different λ values

4. **Actual vs Predicted Values** 
   - Evaluates model prediction quality

---

## 🛠️ Tech Stack

- Python 3.11+  
- NumPy  
- Matplotlib / Seaborn for visualization  
- Pandas for data manipulation  

---

## 📂 Dataset

- Dataset: **House Prices – Advanced Regression Techniques (Kaggle)**  
- Link: [Kaggle House Prices](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)  
- Preprocessing:
  - Selected top features for Linear and Ridge using **Random Forest feature importance**  
  - Normalization/encoding applied as necessary  

---

## 🧮 How It Works

### 1️⃣ Linear Regression
- Initialize weights and intercept
- Update via gradient descent:
w = w - learning_rate * ∂MSE/∂w
b = b - learning_rate * ∂MSE/∂b

###2️⃣ Ridge Regression

Adds L2 penalty to loss function:
Loss = MSE + λ * ||w||²
Gradient descent updates weights accordingly
Coefficient shrinkage visualized across λ

###3️⃣ Lasso Regression
Adds L1 penalty to loss function:
Loss = MSE + λ * Σ|w_i|
Gradient descent updates weights using sub-gradient
Automatically drives unimportant features to zero
Coefficient paths show feature selection effect




Explore polynomial features for non-linear regression
