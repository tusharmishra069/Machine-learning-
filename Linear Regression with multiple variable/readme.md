Linear regression with multiple variables, also known as **multiple linear regression**, is an extension of simple linear regression. It’s used to model the relationship between one dependent variable (target) and multiple independent variables (features). 

### Multiple Linear Regression Equation

In multiple linear regression, the target variable \( y \) is predicted based on a linear combination of multiple predictors \( x_1, x_2, \ldots, x_n \). The general formula is:

\[
y = w_1x_1 + w_2x_2 + \dots + w_nx_n + b
\]

where:
- \( y \) is the predicted value of the target variable.
- \( x_1, x_2, \ldots, x_n \) are the independent variables or features.
- \( w_1, w_2, \ldots, w_n \) are the coefficients (weights) for each feature, representing the impact of each predictor on \( y \).
- \( b \) is the intercept, representing the value of \( y \) when all \( x \)-values are zero.

### Objective of Multiple Linear Regression

The objective is to find the values of \( w_1, w_2, \ldots, w_n \) and \( b \) that minimize the prediction error. This is typically done by minimizing the **Mean Squared Error (MSE)** between the predicted values and the actual values:

\[
MSE = \frac{1}{n} \sum_{i=1}^n (y_i - \hat{y}_i)^2
\]

where:
- \( y_i \) is the actual target value.
- \( \hat{y}_i \) is the predicted target value based on the model.

### Steps in Multiple Linear Regression

1. **Data Collection and Preparation**:
   - Gather and clean your dataset.
   - Separate the target variable \( y \) and the features \( x_1, x_2, \ldots, x_n \).
   - Standardize or normalize the data if features are on different scales.

2. **Model Training**:
   - Use techniques such as **Ordinary Least Squares (OLS)** or **Gradient Descent** to find the optimal values for the weights \( w_1, w_2, \ldots, w_n \) and intercept \( b \).

3. **Prediction**:
   - Once trained, use the model to predict the target variable \( y \) for new data by plugging the values of the features into the equation.

4. **Evaluation**:
   - Measure the performance of the model using metrics such as **Mean Squared Error (MSE)**, **Root Mean Squared Error (RMSE)**, or **R-squared** to evaluate how well the model fits the data.

### Assumptions of Multiple Linear Regression

To achieve reliable results, multiple linear regression assumes:
- **Linearity**: The relationship between each feature and the target variable is linear.
- **Independence**: Observations are independent of each other.
- **Homoscedasticity**: The variance of the residuals is constant across all levels of the independent variables.
- **Normality of Errors**: The residuals (errors) are normally distributed.

### Example of Multiple Linear Regression

Let’s say you want to predict the **price of a house** based on features like:
- \( x_1 \): Square footage
- \( x_2 \): Number of bedrooms
- \( x_3 \): Age of the house

The equation might look like this:

\[
\text{Price} = w_1 \times \text{Square Footage} + w_2 \times \text{Bedrooms} + w_3 \times \text{Age} + b
\]

where the coefficients \( w_1, w_2, w_3 \) reflect the contribution of each feature to the house price.

### Advantages and Limitations

**Advantages**:
- Simple to interpret and implement.
- Can provide insight into the relationships between multiple factors and a target variable.

**Limitations**:
- Assumes linear relationships, which may not hold in real-life data.
- Sensitive to multicollinearity (where predictors are highly correlated with each other), which can skew results.
- Performance can degrade when handling complex, non-linear data.

Multiple linear regression is widely used in fields like finance, economics, and the social sciences, where multiple factors influence the outcome and need to be considered simultaneously.