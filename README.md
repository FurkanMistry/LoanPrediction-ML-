Loan Prediction Based on Customer Behavior
Overview
This project aims to predict the likelihood of customers defaulting on loans based on their demographic and financial information. The dataset used for this project includes features such as income, age, profession, marital status, house ownership status, and more.

Dataset
The dataset used for this project can be found here. It contains information about customers' financial and demographic attributes, including the following features:

Income
Age
Profession
Marital Status
House Ownership Status
Current Job Years
Current House Years
Risk Flag (target variable)
Feature Engineering
Condensing Features
The 'Experience_group' and 'Age_group' columns were condensed into three distinct groups each to simplify the data for subsequent one-hot encoding.
Encoding Techniques
Binary Encoding: Applied for 'Marital_Status' and 'Car_Ownership' columns.
Target Encoding: Used for the 'Profession' feature due to its numerous unique values.
Label Encoding: Employed for 'STATE' and 'CITY' columns to convert them into numeric representations.
One-Hot Encoding: Performed for 'House_Ownership', 'Age_group', and 'Experience_group' columns.
Feature Scaling
MinMaxScaler was applied to numerical features like 'Income', 'CURRENT_JOB_YRS', and 'CURRENT_HOUSE_YRS' to scale them to a similar range.
Model Building
Dataset Balancing
Addressed dataset imbalance using the Synthetic Minority Over-sampling Technique (SMOTE).
Model Evaluation
Evaluated the performance of multiple classification models including Extra Trees, K Nearest Neighbour (KNN), Random Forest, Decision Tree, and Bernoulli Naive Bayes.
Extra Trees emerged as the top performer with an accuracy of 93.21%.
Colab Notebook
Access the Colab notebook for this project here.
