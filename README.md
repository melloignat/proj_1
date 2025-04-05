## **Project description:**

In order to optimize production costs, a metallurgical plant decided to reduce energy consumption at the steel processing stage. We suposed to build a model that would predict the steel temperature of each ladle at the end of each batch. This would allow ladle overheating monitoring and prevent excessive heating to save energy and ultimately - money.

## **Project timeline:**

* EDA and data preprocessing was done. Initially separately for each data source and then processed data was joined to one dataframe for model training. Outliers removed, missing data handled.
* Resulting dataframe was checked for multicollinearity, scaled and some features were removed and some additional custom features added (features engineering)
* Five models were checked - LinearRegression, Ridge, LightGBM, Catboost and RandomForestRegressor
* For each model several hyperparameters were checked through GridSearchCV
* Prediction was done for each model with the best hyperparameters and all models compared via MAE.

## **Project result:**

LightGBM model was selected as the best model and checked on test data. Model MAE on test data was 6.18 and it is less than customer wanted so model was selected as appropriate. Customer will use that model for initial temperature prediction and future tuning (base model).
