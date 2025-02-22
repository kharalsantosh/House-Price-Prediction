# House-Price-Prediction
This repository contains Python implementations for machine-learning problems:
1. **House Price Prediction**: Predicts house prices based on size using linear regression.
2. Why Linear Regression?
Linear regression is a supervised learning algorithm that models the relationship between a dependent variable (
y
y) and one or more independent variables (
x
x). It’s ideal for problems where the relationship is linear.

Steps to Solve the Problem
Define the Model:
y=mx+b
Here:
y = house price,
x = house size,
m = slope (weight),
b = y-intercept (bias).
Loss Function:
We use the Mean Squared Error (MSE) to measure the error:
L(m,b)= 1/N(∑(yi​−(mxi+b))**2 note(i range from 1 to N)

Optimization:
We minimize the loss function using gradient descent. The gradients are:
∂L/∂m=−2/N(i=1∑N(xi(yi−(mxi​+b))
∂L/∂b=−2/N(i=1∑N((yi−(mxi​+b))
Update Parameters:
m_new=m_old−η(∂L/∂m)
b_new=b_old−η(∂L/∂m)
Here, 
η
η is the learning rate.
