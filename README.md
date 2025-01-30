## NLP: Sentiment Analysis on Healthcare Reviews

#### Objective:
  The goal of this project is to develop a model that can classify sentiments in healthcare reviews. This involves analyzing text data from healthcare reviews and determining whether the sentiment expressed in each review is positive, negative, or neutral.

#### Steps involved in this Project:
1. Data Preprocessing
2.  Data Validation
3.  Data Analysis
4.  NLP Pipelines
5.  Model Building
6.  Visulizations
7.  Results

#### Libraries used:
- import pandas as pd
- import numpy as np
- import re
- from nltk.corpus import stopwords
- from nltk.stem.porter import PorterStemmer
- from sklearn.model_selection import train_test_split
- from sklearn.feature_extraction.text import TfidfVectorizer
- from sklearn.linear_model import LogisticRegression
- from sklearn.svm import SVC
- from sklearn.ensemble import RandomForestClassifier
- from sklearn.metrics import accuracy_score, confusion_matrix
- from imblearn.over_sampling import SMOTE
- from wordcloud import WordCloud

#### NLP pipeline:
- Did NLP piplines of Lowering, Stopwords, Stemming
- Used TF IDF vecorizer for conversion of text data to numeric data for model building

#### Visualizations :

- Created  Pie chart, Bar chart , Scatter charts  for distribution of Sentiment data
- Created N-gram chart for getting words which was used mostly
- Word Cloud created to get idea of the textual data

#### Model Building and Evaluation:

- Split the data into train and test set
- Used Logistic Regression, Random Forest Classifier, K-NN ALgorithms to get the accuracy score the data.
- The ACcuracy Score of models are around 0.46 respectively.

#### Challenges:

- There is a data imbalance in target variable/column
- Used SMOTE technique to do over samplimg of the less distributed data.
- After SMOTE , the data got balanced and again build the model with the balanced data
- Accuracy score of Support Vector Machine Algorithm(SVM) and Logistic Regression were around 0.40 after balanced data.

#### Results:
- There is no changes in accuracy level of the models after done SMOTE.
- There is an equal distribution of Bad and Good reviews, comparatively low level of review for neutral review.
- There is no reviews particularly says about Doctor or treatment.
- Most reviews was reagrding staffs, services were highlighted.
- To increase the good reviews of any healthcare induatry,the staffs need to be more patience and need to understand the 
  patient's condition clearly and can act accordingly.
- Healthcare system should be done as service not as business.
  
### Thank you All!
