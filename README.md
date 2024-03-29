# Advertising Budgets and Sales Return  - Multiple Linear Regression

This project delves into the application of multiple linear regression to analyze the intricate relationship between various advertising budgets and sales returns within a business context. The dataset encompasses details on diverse advertising expenses and their corresponding impacts on sales outcomes.

## Multiple Linear Regression

Multiple linear regression is a statistical method used to analyze the relationship between multiple independent variables (features) and a dependent variable (outcome). In contrast to simple linear regression, which considers only one independent variable, multiple linear regression incorporates several predictors to model more complex relationships. The goal is to establish a linear equation that best fits the data, allowing predictions of the dependent variable based on various input features.

### Assumptions

1. Linearity 

The relationship between the independent variables and the dependent variable is assumed to be linear. The model assumes that changes in the independent variables have a constant effect on the dependent variable.

2. Independence

The residuals (the differences between the observed and predicted values) should be independent of each other. In other words, the value of the dependent variable for one observation should not be influenced by the values of other observations.

3. Homoscedasticity

The variance of the residuals should be constant across all levels of the independent variables. This assumption ensures that the spread of the residuals is consistent throughout the range of predictor values.

4. Normality of Residuals

The residuals should follow a normal distribution. This assumption is crucial for hypothesis testing and constructing confidence intervals.

5. No Perfect Multicollinearity

The independent variables should not be highly correlated with each other. High multicollinearity can lead to unreliable estimates of the coefficients.

6. No Autocorrelation of Residuals

The residuals should not exhibit systematic patterns over time or across observations. Autocorrelation could indicate that important information has been omitted from the model.

7. Additivity

The effect of changes in an independent variable on the dependent variable is consistent regardless of the values of other variables. This assumption ensures that interactions between variables are appropriately captured.

### Overfitting

Care should be taken to avoid overfitting by regularization techniques if dealing with high-dimensional data.

### Feature Scaling

Feature scaling may be beneficial for algorithms sensitive to variable scales, in this application it is not necessary.

## Dataset Overview

The dataset captures information related to advertising budgets and their corresponding impact on sales in a business context. It contains the following columns:

1. TV Ad Budget

This column represents the budget allocated for television advertising, indicating the financial resources dedicated to promoting products or services through television channels.

2. Newspaper Ad Budget

This column signifies the budget allocated for newspaper advertising, reflecting the financial investment directed towards advertising in print media.

3. Radio Ad Budget

This column denotes the budget designated for radio advertising, indicating the financial resources allocated for promotional activities through radio channels.

4. Sales

This column represents the sales outcomes, reflecting the actual performance or revenue generated by the business.

In summary, the dataset provides a comprehensive view of advertising expenditures across different media channels (TV, newspaper, and radio) and their corresponding impact on sales.

## Model - ```sklearn.linear_model.LinearRegression```

LinearRegression is a class in the scikit-learn library, designed for linear regression modeling. It provides an implementation of the ordinary least squares (OLS) regression algorithm, making it a fundamental tool for predictive modeling when the relationship between the independent variables and the dependent variable is assumed to be linear.

### Model Performance

- Mean Absolute Error (MAE)

The MAE of 1.04 suggests that, on average, the model's predictions are off by approximately 1.04 units from the actual sales return values. Lower MAE values indicate better accuracy, so a MAE of 1.04 is generally considered good, depending on the scale and context of your sales return values.

- Mean Squared Error (MSE)

The MSE of 1.99 represents the average of squared errors between predicted and actual values. Similar to MAE, lower MSE values are preferred. However, the interpretation is dependent on the scale of your target variable. In this case, a MSE of 1.99 indicates reasonably good model accuracy.

- R-squared (R²)

The R-squared value of 0.89 indicates that approximately 89% of the variability in sales return can be explained by the model. R-squared values range from 0 to 1, where higher values signify better fit. An R² of 0.89 is considered very good and suggests that the model captures a significant portion of the variation in sales returns.

In summary, based on these metrics, the model appears to perform well in predicting sales returns from advertising budgets.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.