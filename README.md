# Customer Churn Prediction for Telco
=====================================
## Introduction
---------------
This project aims to analyze customer behavior and develop a predictive model to identify customers at risk of churning for a home phone and internet service provider, Telco. The goal is to assist Telco in proactively reducing their churn rate and improving customer retention strategies.

## Dataset
------------
The dataset used for this project is the [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) dataset from Kaggle. The dataset consists of 7,043 customer records, each with 20 attributes, including demographic data and account information. The target variable is "Churn," a binary indicator of whether a customer discontinued their service in the previous month.

## Methodology
--------------
1. **Exploratory Data Analysis (EDA)**: The dataset was explored to understand the relationships between features and the target variable.
2. **Data Preprocessing**: The dataset was preprocessed to handle missing values, convert categorical variables, and scale numerical features.
3. **Feature Selection**: A chi-squared test was used to select the most relevant features for the model.
4. **Modeling**: Several classification models were trained and evaluated, including logistic regression, random forest, and support vector machine (SVM).
5. **Hyperparameter Tuning**: Grid search was used to optimize hyperparameters for the models.
6. **Model Evaluation**: The performance of each model was evaluated using metrics such as accuracy, precision, recall, F1 score, and area under the curve (AUC).

## Results
------------
The results of the analysis are as follows:
* The logistic regression model with SMOTE (Synthetic Minority Over-sampling Technique) and feature selection achieved the highest AUC score of 0.832.
* The most influential predictors of customer churn were:
	+ Tenure
	+ MonthlyCharges
	+ InternetService
	+ Contract type
* Customers on month-to-month contracts, using fiber optic services, with higher monthly charges, and less than 18 months of tenure were more likely to churn.

## Conclusion
------------
The analysis suggests that Telco can reduce customer churn by targeting customers with specific characteristics, such as those on month-to-month contracts, using fiber optic services, with higher monthly charges, and less than 18 months of tenure. The logistic regression model with SMOTE and feature selection can be used to predict customer churn and inform retention strategies.

## Recommendations
------------------
1. **Targeted Marketing**: Telco can develop targeted marketing campaigns to retain customers with high churn risk.
2. **Contract Optimization**: Telco can offer customized contract options to customers with high churn risk.
3. **Service Improvement**: Telco can improve its services, such as internet speed and reliability, to reduce customer dissatisfaction and churn.
4. **Customer Engagement**: Telco can increase customer engagement through regular communication, surveys, and feedback mechanisms to identify and address customer concerns.

## Future Work
-------------
1. **Collect Additional Data**: Collect more data on customer behavior, such as usage patterns and customer feedback.
2. **Experiment with New Models**: Experiment with new machine learning models, such as neural networks and gradient boosting.
3. **Hyperparameter Tuning**: Perform hyperparameter tuning for the models using techniques such as Bayesian optimization.
4. **Model Deployment**: Deploy the model in a production environment to predict customer churn and inform retention strategies.
