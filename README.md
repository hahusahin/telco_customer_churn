# Telco Customer Churn Detection by Using Classification

### Goal
The goal of this analysis is to predict the churning customers by using machine learning algorithms of classification.

### Data Description
* The dataset has a total of 7043 observations with 21 variables.

* Total number of features are 20, of which 4 is quantitative and 16 categorical.

* Target variable is the binary variable of Churn that shows whether the customer left within the last month.

### Exploratory Data Analysis
* Missing values are detected and filled, unnecesarry features are deleted

* Target variable's distribution is examined

* Relationship between target variable and the features are examined and some observations are made

* Outliers are checked

* Scaling is applied as some classification algorithms are sensitive to it.

### Modeling
* Data is splitted into train and test set.

* 6 models (Logistic Regression, K-Nearest Neighbors, Random Forest, Support Vector Machine, XGBoost, Light GBM) are selected, base model is built for each and then these models are improved by hyperparameter tuning.

* Since data is mildly imbalanced (has a churning rate of 26%), Stratified Sampling is applied while splitting and relevent parameters (giving weight to classes) are used while hyperparameter tuning
    
* While taking Accuracy score into consideration, F1 score is chosen as the first performance evaluation metric since our data is imbalanced. 

* In conclusion, the winner of this classification problem is XGBoost Model as it has the best F1 score and a good accuracy.

### Files
* Telco_Customer_Churn.csv - Data set
* telco_churn.ipynb - Project Notebook

### Libraries Used
* pandas, numpy
* matplotlib, seaborn
* sklearn
* xgboost, lightgbm
