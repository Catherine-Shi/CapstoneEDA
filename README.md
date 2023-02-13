## Summary Overview 
### Business Problem  
This file focuses on exploring US healthcare costs. Healthcare cost is a significant expense for most people and companies. Fitting a model for estimating healthcare costs can help businesses and individual family manage their expense for future years and expect fewer high-cost surprises.
### Dataset
This dataset contains 1338 rows of insured data, where the Insurance charges are given against the following attributes of the insured: Age, Sex, BMI, Number of Children, Smoker, and Region. There are no missing or undefined values in the dataset. This dataset is helpful in understanding the risk underwriting in Health Insurance, the interplay of various attributes of the insured, and seeing how they affect the insurance premium.
### EDA Analysis 
Through preliminary eda analysis, we led to the conclusion that smokers and the older population tend to receive higher insurance charges compared to non-smokers and the younger population. There are no significant differences in costs in terms of different sex, region, and the number of children in the household. To better fit the model, dummy variables are produced for categorical columns, and log transformation is applied to normalize specific data. Various plots are displayed in this section to provide further details.
### Baseline model 
To set a rule for determing the performance of models, a baseline model is built using a dummy classifier strategy. The model generates 0.85 MSE for training data and 0.88 MSE for testing data. Models should at least perform better than the baseline model to be considered to be a good one.
### Models used 
For this problem, we used models including linear regression, lasso regression, ridge model, and sequential Feature selection model. Mean squared error scores for both testing and training data are used to compare the performance of each model. Training time are also taken into consideration.
### Model Improvement 
After applying the simple model, further features are explored using GridSearchCV in trying different parameters for the models. From the results, we find that the ridge model is best performed with an alpha of 1; and the sequential feature selection model's best parameter is 5. A summary detail is displayed at the end of the file for a clearer view.
### Results 
Given the training time and MSE scores, all models perform better than the baseline model. Among all of them, the linear regression model and ridge model may be the better choice for future exploration of this problem. Sequential Featuer selector, although it does perform good results, takes up a longer training time than the other models.
