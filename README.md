# 02_Linear_Regression_Multi_Dimensional

Linear Regression is a foundational algorithm in supervised machine learning, used to predict a continuous target variable by modeling a linear relationship between input features and the target.

## What is Multi-Dimensional Linear Regression?
Multi-Dimensional Linear Regression, also known as Multiple Linear Regression, extends the concept of simple linear regression to include multiple independent variables (features). It aims to find a linear relationship between multiple input features $X$ and the target variable $y$.

### Key Features
1. **Supervised Learning**: It learns from labeled data, establishing a relationship between input features and the output target.
2. **Regression Task**: Predicts numerical (continuous) values, such as house prices, sales, or temperatures.

## The Linear Relationship
The equation for multi-dimensional linear regression is:

```math
y = \beta_0 + \beta_1x_1 + \beta_2x_2 + \dots + \beta_nx_n + \epsilon
```

Where:
- $y$ : Target variable (what we want to predict).
- $\beta_0$ : Intercept (value of $y$ when all $x_i = 0$).
- $\beta_1, \beta_2, \dots, \beta_n$ : Coefficients (impact of each feature on $y$).
- $x_1, x_2, \dots, x_n$ : Independent variables (features).
- $\epsilon$ : Error term (captures noise not explained by the model).

## Key Concepts

### Dependent and Independent Variables
- **Independent variables $x_i$** : Input features (e.g., area, number of rooms).
- **Dependent variable $y$** : Output/target (e.g., house price).

### Line of Best Fit
The model finds the line (or hyperplane in higher dimensions) that minimizes the sum of squared residuals (differences between predicted and actual values).

### Assumptions of Linear Regression
1. **Linearity**: The relationship between features and the target is linear.
2. **Homoscedasticity**: Errors have constant variance across all levels of $x$.
3. **Independence**: Observations are independent.
4. **Normality**: Errors are normally distributed.

## Example: House Price Prediction
Suppose you work for a real estate company and want to predict house prices based on several features:
- **Area** (in square feet)
- **Number of bedrooms**
- **Location score**

Using Multi-Dimensional Linear Regression, you might get an equation like:
```math
\text{Price} = 50,000 + 150(\text{Area}) + 10,000(\text{Bedrooms}) + 5,000(\text{LocationScore})
```

### Interpretation
- A base price of $50,000 is added for any house.
- For every additional square foot, the price increases by $150.
- Each additional bedroom adds $10,000 to the price.
- Higher location scores contribute $5,000 per unit.

## Advantages
- **Handles multiple input features**, enabling more accurate predictions.
- **Easy to interpret** when assumptions are met.

## Applications
- **Real estate price prediction**.
- **Forecasting sales or revenue**.
- **Analyzing the impact of multiple factors** in scientific studies.

Explore the notebooks in this repository to see how multi-dimensional linear regression is implemented both from scratch and using Scikit-learn!

