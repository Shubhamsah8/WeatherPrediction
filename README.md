# WeatherPrediction
This project focuses on utilizing the Rainfall in Australia dataset to predict whether it will rain tomorrow. 
Various machine learning models such as CatBoost, XGBoost, Random Forest, and Support Vector Classifier were tested extensively. 
Among these models, CatBoost exhibited exceptional performance, achieving an impressive AUC score and ROC score of 89, surpassing the performance of the other models. 
However, due to limited system compatibility, hyperparameter tuning was not conducted. Nevertheless, it is highly recommended to perform hyperparameter tuning if feasible.

# Tech Stack
* Front-End: HTML, CSS, Bootstrap
* Back-End: Flask
* IDE: Jupyter notebook, Spyder

# How to run this app
* First create a virtual environment by using this command:
* conda create -n myenv python=3.8
* Activate the environment using the below command:
* conda activate myenv
* Then install all the packages by using the following command
* pip install -r requirements.txt
* Now for the final step. Run the app
* python app.py


# Workflow

# Data Collection: 
[Rainfall Prediction in Australia dataset](https://www.kaggle.com/jsphyg/weather-dataset-rattle-package) from Kaggle
# Data Preprocessing: 
* Missing Values Handled by Random Sample imputation to maintain the variance
* Categorical Values like location, wind direction are handled by using Target guided encoding
* Outliers are handled using IQR and boxplot
* Feature Selection and was done but didnt perform well it can be seen in testing_notebook/Prediction.ipynb
* Feature Scaling didnt give a lot of difference it also can be seen in testing_notebook/RainPrediction1.ipynb
* Imbalanced Dataset was handled using SMOTE
# Model Creation:
* Different types of models were tried like catboost, random forest, logistic regression, xgboost, support vector machines, knn, naive bayes.
* Out of these catboost, random forest and support vector machines were top 3
* The conclusion were made using classification metrics. roc curve and auc score
