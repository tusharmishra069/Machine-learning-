# Linear Regression

Linear regression is a fundamental algorithm in machine learning, primarily used for predictive modeling. It establishes a linear relationship between a dependent variable (target) and one or more independent variables (predictors) by fitting a straight line (or hyperplane in multiple dimensions) to the data. The goal is to predict the output for a new input based on this linear relationship.

## Key Concepts in Linear Regression

### Simple vs. Multiple Linear Regression

**Simple Linear Regression:** Involves a single predictor variable. The relationship is defined by the equation:

 y = mx + b


where  y  is the predicted target,  m is the slope indicating how much  y  changes with x , and b  is the intercept.

**Multiple Linear Regression:** Extends this concept to multiple predictors, with the formula:
y = w_1 x_1 + w_2 x_2 + ..... + w_n x_n + b 
where x_1, x_2, ..... x_n  are predictors,w_1, w_2, .... w_n are weights, and \( b \) is the intercept.

### Objective

The aim is to minimize the difference between the actual and predicted values by adjusting the line or plane's slope and intercept. This is often achieved by minimizing the Mean Squared Error (MSE):
\[ MSE = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 \]
where \( y_i \) are the actual values, and \( \hat{y}_i \) are the predicted values.

### Gradient Descent

Linear regression often uses gradient descent, an optimization algorithm, to minimize the error by iteratively adjusting weights and the intercept based on the gradient of the error function.

### Assumptions

- **Linearity:** There is a linear relationship between predictors and the target.
- **Independence:** Observations are independent of each other.
- **Homoscedasticity:** The residuals (errors) have constant variance.
- **Normality:** The residuals are normally distributed.

## Applications

Linear regression is widely used in forecasting, risk analysis, and other fields where prediction of a continuous outcome is desired, such as predicting house prices based on features like size and location.

## Advantages and Limitations

**Advantages:**
- Simple and easy to interpret.
- Requires less computational power.

**Limitations:**
- Sensitive to outliers.
- Assumes a linear relationship, which may not hold for complex datasets.

Linear regression remains an essential tool for understanding relationships in data, often serving as a foundation before moving to more complex algorithms.
