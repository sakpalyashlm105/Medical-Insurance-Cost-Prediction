# Medical-Insurance-Cost-Prediction

This project looks at predicting individual medical insurance costs using machine learning techniques. The goal is to understand what factors influence medical insurance costs and build models to accurately predict costs given details like a person's age, BMI, smoking status etc.

## Data
The dataset used is originally from Kaggle: https://www.kaggle.com/mirichoi0218/insurance

It contains 1338 rows with the following attributes:

* age: age of primary beneficiary
  
* sex: insurance contractor gender, female, male
  
* bmi: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height, objective index of body weight (kg / m ^ 2) using the ratio of height to weight, ideally 18.5 to 24.9
  
* children: Number of children covered by health insurance / Number of dependents
  
* smoker: Smoking
  
* region: the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.
  
* charges: Individual medical costs billed by health insurance

## Analysis
The analysis focused on using machine learning techniques like KNN, Linear Regression, Decision Trees, Random Forests and XGBoost to predict the charges variable given the other attributes.

The steps included:

* Data import and inspection
* Exploratory data analysis
* Preprocessing like encoding categorical variables
* Train-test split
* Model building and hyperparameter tuning for the algorithms
* Quantifying performance using RMSE and other metrics
* Feature importance analysis

## Results
XGBoost proved to give the best performance with a test RMSE of 4304, compared to poor performance from a baseline KNN model with 12,150 RMSE. Feature importance analysis using SHAP values also provided interesting insights on how different attributes impact the prediction.

The other models tried and their performance:

* KNN: 12,150 RMSE
* Linear Regression: 5,975 RMSE
* Decision Tree: 4,485 RMSE
* Random Forest: 4,297 RMSE
