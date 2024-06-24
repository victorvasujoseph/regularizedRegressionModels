# Regularized Regression Models
Selecting features using ridge regularization, LASSO regularization, and sequential feature selection

This activity is meant to summarize the work with regularized regression models. 

We will build regression models to predict wage. Incorporate the categorical features and transform the target using a logarithm.  We will also Build ridge models and consider different amounts of regularization. After fitting the model, we will interpret it and try to understand what features led to higher wages.

We will use the sklearn data set.

wages = fetch_openml(data_id=534, as_frame=True)

Ridge Regression MSE: 22.324511499518042
LASSO Regression MSE: 32.94700199282025

# Learning and Conclusion

## Regularization:

Both Ridge and LASSO regression apply regularization to prevent overfitting.
Ridge regression tends to shrink coefficients towards zero, while LASSO regression can set some coefficients to zero, effectively performing feature selection.

## Log Transformation:

Transforming the target variable (wage) using a logarithm helps stabilize variance and make the data more normally distributed, improving model performance.

Feature Importance:

Permutation importance provides insights into which features are most influential in predicting wages.
Features such as education and occupation have significant importance.
Model Comparison:

Ridge regression had a lower MSE compared to LASSO regression in this case, indicating it might be a better fit for this dataset.
