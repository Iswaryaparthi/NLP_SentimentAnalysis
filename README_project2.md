# FinalProject
## Project 2 - Predicting Hospital Readmissions

#### Objective:

  The primary goal of this project is to build a predictive model that can identify patients who are at high risk of hospital readmission within 30 days after their initial discharge.

#### Tasks carried out in this project:

- Importing libraries
- Data Collection and Preprocessing
- Feature Engineering
- Model Building
- Model Evaluation
- Visualizations
- Challenges
- Results and Insights

#### Libraraies to Import:

- import pandas as pd
- import numpy as np
- import seaborn as sns
- import matplotlib.pyplot as plt
- from sklearn.preprocessing import LabelEncoder
- from sklearn.model_selection import train_test_split
- from sklearn.tree import DecisionTreeClassifier
- from sklearn.ensemble import RandomForestClassifier
- from sklearn.svm import SVC
- from sklearn.linear_model import LogisticRegression
- from sklearn.metrics import confusion_matrix, accuracy_score, classification_report

#### Data Collection and Preprocessing:

- Get the data as csv,xlsv file format
- Check the data for null values, dupliactes, distribution of the data
- Get the statistics of the data
- The given data is a mixture of categorical and continuous
- Convert the categorical data into numeric data using encoders like label, ordinal, one-hot encoders

#### Feature Engineering:

- After the data conversion, again check for null, missing, duplicate values
- Select the features which is going to help to create model building
- In this dataset there are 13 column with 1000 rows data
- From that I took Readmitted as target column and others are as independent variable
- Check for any outliers in the selected features, if there is any outliers persist try to fill it or delete it based on the project 
  needs and importance of the particular feature.

#### Visualizations:

- Build correlation matrix using  heatmap to find the correlation of the variables with target variable
- Histogram, Box plot, Countplot are used to get the distribution of the individual features
- Boxplot, Barplot to get the realtionship among feature and target variable

#### Model Building & Model Evaluation:

- After feature engineering and visualizations will get the idea to select the X and y variable to do model building
- I used Decision tree Classifier, Random tree Classifier, Support Vector Machines, Logistic Regression for model building
- I tried with the combination for 3-4 features as X variable and y as Readmitted column several times with all the models
- I got the accuracy score ranging from 0.43 to max of 0.53
- In order to increase the accuracy of the model , I did parameter tuning for Random tree classifier and got the same score as 0.53

#### Challenges:
- No data regarding patient admission date or discharge date
- Outliers detected in Age column
- No changes happened after trying to fill with either mean or median
- Low accuracy score determined

#### Results and Insights:

- The number of patients readmitted again is equal as who dnt readmitted again 
- Age,Num_Medications, Num_Emergency_Visits, Number of diagnoses provided the more information readmission status
- Taking two features to build a model gives an better result
- Diabetics, Heart Patients have a very slight increase of readmission status

#### Thank you All!


   




