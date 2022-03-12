# Supervised Machine Learning Analysis - Predicting Credit Risk

In this analysis, I built a machine learning model that attempts to predict whether a loan from LendingClub will become high risk or not.

**Background**

LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.
I will be using this data to create machine learning models to classify the risk level of given loans. Specifically, I will be comparing the Logistic Regression model and Random Forest Classifier.

**Retrieve the data**

I downloaded data from LendingClub and output two CSVs:

2019loans.csv
2020Q1loans.csv

**Preprocessing: Convert categorical data to numeric**

I created a training set from the 2019 loans using pd.get_dummies() to convert the categorical data to numeric columns. Similarly, I created a testing set from the 2020 loans, also using pd.get_dummies().

![Screen Shot 2022-03-12 at 2 10 53 PM](https://user-images.githubusercontent.com/87212158/158031622-a3c8af13-253e-4898-a4af-dce6ab5c0615.png)

**Hypothesis - Consider the models**

I included a prediction as to which model I thought would perform better.

**Fit a LogisticRegression model and RandomForestClassifier model**

I created a LogisticRegression model, fit it to the data, and printed the model's score. I also repeated the process for a RandomForestClassifier. 

![Screen Shot 2022-03-12 at 2 11 44 PM](https://user-images.githubusercontent.com/87212158/158031653-7ad69c21-97be-414f-aa5e-dd6a9efc12ed.png)

**Revisit the Preprocessing: Scale the data**

Using StandardScaler I scaled the training and testing sets. Then I fit and scored the LogisticRegression and RandomForestClassifier models on the scaled data. 

![Screen Shot 2022-03-12 at 2 12 07 PM](https://user-images.githubusercontent.com/87212158/158031667-4c151636-0c10-4a77-a937-b0f17381812d.png)
