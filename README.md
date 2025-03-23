## **Project description**

Project to help steel plant to analyse and predict ladle temperature at the end of the production line to save costs on ladle heating.

Project is made with **Python** and in **Jupyter Notebook** format.

<hr>

### **Main task**

In order to optimize production costs, some metallurgical plant decided to reduce energy consumption at the steel processing stage. We suposed to build a model that would predict the steel temperature of each ladle at the end of each batch. This would allow ladle overheating monitoring and prevent excessive heating to save energy. We do have the following data to begin with:

### **Data description**

Data consists from files received from various sources:

* **data_arc_new.csv** — data about electrodes;
* **data_bulk_new.csv** — data about the supply of bulk materials (volume);
* **data_bulk_time_new.csv** — data about the supply of bulk materials (time);
* **data_gas_new.csv** — data on gas blowing through the alloy;
* **data_temp_new.csv** — data about temperature measurement;
* **data_wire_new.csv** — data about wire material (volume);
* **data_wire_time_new.csv** — data about wire material (time);

### **Project timeline:**
* EDA and data preprocessing was done.Initially separately for each data source and then processed data compiled for model training. Outliers removed, missing data handled.
* Joined data was checked for multicollinearity, scaled and some features were removed and some custom features added (**features engineering**)
* Five models were checked - **LinearRegression**, **Ridge**, **LightGBM**, **Catboost** and **RandomForestRegressor**
* For each model several hyperparameters were checked through **GridSearchCV**
* Prediction was done for each model with the best hyperparameters and all models compared via **MAE**.
* LightGBM was selected as the bst model and checked on test data
* **Best model MAE on test data was 6.18** and it is less than customer wanted so model was selected as appropriate.

<hr>
