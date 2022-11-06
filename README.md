# Homework 19 - Supervised Machine Learning

### Background

"Lending services companies allow individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. This data will be used to determine whether a borrower is creditworthy and should be issued a loan.
You will be using this data to create machine learning models to classify the risk level of given loans. Specifically, you will be comparing the Logistic Regression model and Random Forest Classifier."


### Prework predictions

Before beginning work on running the models for this assignment (logistical regression and random forest classifier), my prediction is that the logistic regression model will perform better. Since the dataset has a relatively simple categorical variable - determining if a loan is approved or not - a logistical regression model is designed for this type of task. Random forest models are more effective when there are more categories to classify, so I believe that the logistical regression will perform better.

### Process

1. Imported the data `lending_data.csv`.
2. Defined the X and y variables. 'y' is the value of the "loan_status" column and 'X' is the data from the rest of the dataset, minus the "loan_status" column.
3. Used the `train_test_split` sklearn function to prepare the data.
4. Began testing the Logistic Regression model by importing the sklearn `LogisticRegression` function.
5. Created a classifier and fit the data with *X_train* and *y_train*.
6. Validated the model with the test data.
7. Ran predictions and received a training data score of **0.9921** and a test data score of **0.9918**.
8. Began testing the Random Forest Classifier Model by importing the sklearn `RandomForestClassifier` function.
9. Imported the sklearn `StandardScaler` function and fit the X_train data.
10. Scaled and transformed the X_train and X_test data.
11. Ran the Random Forest Classifier and received a training data score of **0.9975** and a test data score of **0.9917**.

### Postwork analysis
After importing the data and running the models, the results show very similar and close scores for both the logisitc regression and random forest classifier. The test scores for both models had a 0.0001 difference, which is very close to similar results. As such, I think that both models work well when there is a binary choice in results, such as yes or no, and neither is the wrong choice.
