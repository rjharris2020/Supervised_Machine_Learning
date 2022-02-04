# Predicting Credit Risk

## In this assignment, I will be building a machine learning model that attempts to predict whether a loan from LendingClub will become high risk or not.

### Retreive the data 
In the Generator folder in Resources, there is a GenerateData.ipynb notebook that will download data from LendingClub and output two CSVs:

2019loans.csv
2020Q1loans.csv

I will be using an entire year's worth of data (2019) to predict the credit risk of loans from the first quarter of the next year (2020).

### Preprocessing: Convert categorical data to numeric
Create a training set from the 2019 loans using pd.get_dummies() to convert the categorical data to numeric columns. Similarly, create a testing set from the 2020 loans, also using pd.get_dummies(). 

### Consider the models
I will be creating and comparing two models on this data: a logistic regression, and a random forests classifier. Before I create, fit, and score the models, I need to make a prediction as to which model I think will perform better. 

### Fit a LogisticRegression model and RandomForestClassifier model
Create a LogisticRegression model, fit it to the data, and print the model's score. Do the same for a RandomForestClassifier. 

### Revisit the Preprocessing: Scale the data
The data going into these models was never scaled, an important step in preprocessing. Use StandardScaler to scale the training and testing sets. Before re-fitting the LogisticRegression and RandomForestClassifier models on the scaled data, make another prediction about how scaling will affect the accuracy of the models. 

Fit and score the LogisticRegression and RandomForestClassifier models on the scaled data.
