# Marketing-Department
Regression, customer segmentation of a Marketing Dataset

- We identified the customers who spend more and those who spend less(spender vs saver) - Customer Segmentation
- We performed Linear Regression to predict 'PURCHASES'
- We performed Random Forest Regressor to predict 'PURCHASES'.
- We did PCA on our dataset to reduce the dimensionality
- We observed the improvement in Random Forest Regressor with 50 and 100 Trees
- We compared our models
Our analysis was based on analyzing customer behaviors and developing predictive models to predict Purchases.

1. Customer Segmentation

- We first performed customer segmentation on our data to find those who spend(spenders) and those who save(savers). This helped us understand the distribution and characteristics of our dataset.

2. Linear Regression

- We then set out to predict the 'PURCHASES column using Linear Regression. We observed the performance of our model on scaled and unscaled data. The model performed better with scaled data.
- With Linear Regression the model had a high R squared value indicating its predicting power. But the MSE values were relatively low if you look at the range of the PURCHASES Feature.
- We then looked at Residual Plots, to check for the distribution among the errors. The errors were found around zero with few outliers. This indicates that our erros are random and do not follow any pattern
- We then found the Feature Importance from the coefficients of Linear Regression and observed, ONEOFF_PURCHASES and INSTALLMENTS_PURCHASES were the most significant predictors and Features like CASH_ADVANCE_FREQUENCY and PURCHASES_FREQUENCY showed a significant negative impact, indicating an inverse relationship with the target variable.
- We also performed Principal Component Analysis(PCA). This reduces the dimensionality of our dataset and we can visualize the patterns.
- Upon performing PCA we can notice that our data forms clusters. Running Clustering models on such a dataset would be a good idea
- 
3. Random Forest Regressor

- We then performed Random Forest Regressor on our scaled data, we observed the improvement in prediction with the increase in number of trees from 50 to 100.
- The random forest regressor achieved a high R squared value, indicating its ability to explain the variance in the target feature (PURCHASES)
- The MSE values are relatively high when you look at the range of PURCHASES column
- The MSE values are higher compared to our Linear Regression model

### On comparing the results between Linear Regression and Random Forest Regressor we can say that our Linear Regression Model makes more accurate predictions and is the best choice for our dataset
