# Logistic Regression

## Assignment Information

- **Student Name:** Mpayimana Cyiza Landry
- **Assignment Title:** Logistic Regression
- **School:** Stanford University
- **Course:** Supervised Machine Learning: Regression and Classification

---

## Assignment Overview

In this practice lab, I implemented logistic regression from scratch to solve two classification problems: predicting student admission based on exam scores, and predicting microchip quality based on test results. The assignment covered both regularized and non-regularized logistic regression, feature mapping, and decision boundary visualization.

---

## What I Learned

### 1. **Logistic Regression Fundamentals**
- Understood the sigmoid function and its role in binary classification
- Learned the logistic regression model: `f_w,b(x) = g(w·x + b)`
- Implemented the cost function for logistic regression
- Understood the gradient descent algorithm for logistic regression

### 2. **Sigmoid Function**
- Implemented the sigmoid function: `g(z) = 1/(1+e^(-z))`
- Understood the output range (0 to 1) as probability
- Learned to apply sigmoid to both scalars and arrays

### 3. **Cost Function and Gradient**
- Implemented the binary cross-entropy loss function
- Derived and implemented gradient formulas
- Understood the relationship between predictions and errors

### 4. **Regularization**
- Implemented L2 regularization to prevent overfitting
- Added regularization term to cost function
- Modified gradient descent with regularization
- Understood the trade-off between model complexity and generalization

### 5. **Feature Engineering**
- Implemented polynomial feature mapping for non-linear decision boundaries
- Transformed 2 features into 27 polynomial features
- Understood how feature mapping enables more complex models

### 6. **Model Evaluation**
- Implemented prediction function with 0.5 threshold
- Calculated training accuracy
- Visualized decision boundaries

---

## What I Accomplished

### ✅ Implemented Core Functions

1. **`sigmoid(z)`**
   - Computed sigmoid function for scalars and arrays
   - Handled vectorized operations

2. **`compute_cost(X, y, w, b)`**
   - Computed logistic regression cost function
   - Used binary cross-entropy loss
   - Handled multiple training examples

3. **`compute_gradient(X, y, w, b)`**
   - Computed gradients for gradient descent
   - Returned both `dj_db` and `dj_dw`

4. **`predict(X, w, b)`**
   - Made predictions using 0.5 threshold
   - Returned binary predictions (0 or 1)

5. **`compute_cost_reg(X, y, w, b, lambda_)`**
   - Added L2 regularization term to cost function
   - Controlled overfitting

6. **`compute_gradient_reg(X, y, w, b, lambda_)`**
   - Added regularization to gradient
   - Updated weight updates with `lambda_/m * w_j`

### ✅ Built Complete Models

**Part 1: Student Admission Classifier**
- **Dataset**: 100 examples (2 features: exam scores)
- **Model**: Logistic regression without regularization
- **Accuracy**: ~92%
- **Application**: Predict admission based on exam scores

**Part 2: Microchip Quality Classifier**
- **Dataset**: 118 examples (2 features: test results)
- **Feature Mapping**: 2→27 polynomial features
- **Model**: Regularized logistic regression
- **Accuracy**: ~80%
- **Application**: Predict microchip acceptance/rejection

### ✅ Achieved Understanding

- Discovered the importance of regularization in preventing overfitting
- Learned how feature mapping enables non-linear decision boundaries
- Understood the effect of lambda on model complexity
- Visualized decision boundaries for both linear and non-linear classifiers

---