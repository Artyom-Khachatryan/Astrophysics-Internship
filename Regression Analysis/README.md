I Use visualization methods like box plots and histograms, those helps understand the dataset more correctly.Correlations between variables like tip, size, and total_bill is higher, which means total_bill and size can have large impact of model performance. For checking I drop all categorical features from dataset, and seeing that model performance isn't decrease much.
Employing different regression models like Linear Regression, Lasso, etc., with various loss functions provides insight into model performance.Best scores in terms of mse,mae and r2 score I have in the case of use ElasticNet. Evaluating with these metrics is good for more detail model understanding: MSE is more sensitive to outliers than MAE, and using these metrice together is good for understanding impact of outliers in model performance.R2 scores range between 0 and 1, providing more informative insights for people to understand model performance. I tried using boosting algorithms as well, but their performance didn't meet expectations.

Linear Regression: 
   Mean Squared Error: 0.6683
   Mean Absolute Error: 0.6604
   R2 Score: 0.4652

Lasso: 
   Mean Squared Error: 0.5665
   Mean Absolute Error: 0.6256
   R2 Score: 0.5467

ElasticNet:
   Mean Squared Error: 0.56381
   Mean Absolute Error: 0.6231
   R2 Score: 0.5489

AdaBoost:
   Mean Squared Error: 0.9088
   Mean Absolute Error: 0.7980
   R2 Score: 0.2728
