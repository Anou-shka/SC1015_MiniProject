
# SC1015 Mini-Project 

by Anoushka, Dominick and Yojin 
  
## Dataset- Loan Prediction Analysis by Debdatta Chatterje
Published on Kaggle

### Introduction
In this project we will be predicting the loan_status of the project with the help of various numerical and categorical variables like Gender, CoapplicantIncome and Loan_Amount_Term etc. We will be using two machine learning models in predicting the loan_Status and compare their accuracy to tell which is a better model.

### Cleaning of the dataset
We will be removing the null cells and replacing them with their median to provide better answer for the solution.
We included dummy variables into the dataset so as to be able to use these categorical variables as predictors. This was done by splitting the categorical variables for example property areas into multiple binary columns, assigning a value to each categories

### Exploratory Data Analysis
In EDA, we will be analysed each variables from the data set. We used graphs comparing Loan_Status against the different categorical variables and show the percentage of loan_status approved or not. Futhermore, we also used boxplot and stripplot to visualize the effect of ApplicantIncome and CoapplicantIncome on the approval of loan.

### Logistic Regression
We used logistic regression to predict the loan_status. We will be working with LogisticRegression function imported from sklearn.

In this method, we dropped Loan_ID as it does not affect the loan_status. We will also be dropping loan_status as targetted variables needs to be in a separate dataset. Thereafter, we will use dummies function to convert categorical variables into binary values and then fit the logistic regression model. We then split the dataset into train and test set, the same train and test set will also be used in Decision tree.

We then proceed by predicting with the train set created after train_test_split. Afterwhich, we predict the loan_status and check the accuracy score and goodness of fit of the train and test data.

The classification accuracy was around 0.85 and 0.76 for train and test data respectively.

### Decision Tree
We also used decision tree we use to predict the loan_status. We will be working with DecisionClassifier which has also been imported from sklearn. We used the same train and test set for both the methods so as be able to compare the accuracy score of both model.

After fittng the model, we predicted loan approval of each applicant. We then plot the decision tree and generated a heat map for the outcome.

The classification accuracy score for the decision tree was 0.83 and 0.77 for train and test data repectively.

### Conclusion
From our exploratory data analysis we saw that we have balanced number of numerical and categorical independent variables, in addition, our data set have showed that the independent variables were able to be relatively linearly separable with distinct partition. 
However, due to the greater ease of visualizing the data, we conclude that decision tree would be the preferred model
