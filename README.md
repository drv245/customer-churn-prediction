# Customer Churn Prediction

This is a machine learning project that predicts whether a telecom customer will leave (churn) or stay.

## Project Summary
I built two models which are Logistic Regression and Decision Tree to predict whether a telecom customer will churn (leave) or stay.

## Data
- The dataset has 7043 customers and 21 columns.
- 73.5% of customers stayed and 26.5% left.
- I fixed the TotalCharges column, which was stored as text and not numbers as it should be numeric.
- changed the text columns into numbers using .map() for individual columns and get_dummies() for multiple columns.
- I split the data 80/20 into training and test sets, keeping the same share of leavers in both.

## Models and Results
- Logistic Regression: accuracy 81%, recall 56% (209 of 374 leavers caught)
- Decision Tree: accuracy 79%, recall 54%
- Now on comparing these two models we can see Logistic Regression performed better!

## Key Finding
Accuracy looked good at 81%, but recall was only 56%.
This means the model missed almost half of the customers who left.
This is a problem because the company loses customers it could have kept.

## Tools Used
- Python and Pandas
- Scikit-learn (LogisticRegression, DecisionTreeClassifier, confusion matrix, classification report)
- Jupyter Notebook
