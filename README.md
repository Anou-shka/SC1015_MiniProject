
# SC1015 Mini-Project 

by Anoushka, Dominick and Yojin 
  
## Dataset- Loan Prediction Analysis by Debdatta Chatterje
Published on Kaggle 
 
### Introduction 
 
In this project we will be predicting the loan_status of the project with the help of various numerical and categorical variables like Gender, CoapplicantIncome and Loan_Amount_Term etc. We will be using two machine learning models in predicting the loan_Status and compare their accuracy to tell which is a better model. 

### Cleaning of the dataset

We will be removing the null cells and replacing them with their median to provide better answer for the solution. 

### Exploratory Data Analysis 

In EDA, we will be comapring variables of train data set. There are graphs representing Loan_Status will different categorical variables and show the percentage of loan_status approved or not. 
Futhermore, we have boxplot and stripplot representing ApplicantIncome and CoapplicantIncome with the loan_status showing which should be the minimun and maximum income which will be approved. 

### Logistic Regression 

This will be the first method used to predict the loan_status. We will be working with LogisticRegression which has been imported from sklearn. 

In this method, we will drop Loan_ID as it does not affect the loan_status. We will also be dropping loan_status as targetted variables needs to be in a separate dataset. Thereafter, we will use dummies function to convert categorical variables into binary values and then fit the logistic regression model. Before this, we will split the dataset into train and test set, which will also be used in Decision tree. 

We will proceed by predicting with the train set created after train_test_split. Then will predict the loan_status and check the accuracy score and goodness of fit of the train and test data. 

The accuracy was around 0.82 and 0.79 for train and test data respectively. 

### Decision Tree 

This will the second method we use to predict the loan_status. We will be working with DecisionClassifier which has also been imported from sklearn. Also, we will be using the same variables from train_test_split so the data set remains the constant for both the methods and the accuracy score is compareable. 

After fittng the model, we will be predicting with variables of train_test_split. Then, plotting the decision tree from train_test_aplit variables and predictors variables. We will also be checking the goodness of fit and classification accuracy of both train and test data after predicting the loan_status. 

The accuracy score for the decision tree was 0.83 and 0.79 for train and test data repectively. 

### Conclusion 

Decision/Classification tree would be better in predicting the loan_status as we had more categorical variables than numerical variables and the relationship would likely more complex than linear due to external factors. 

Lastly, Decision Tree is easier to visualize than Logistic Regression. 
