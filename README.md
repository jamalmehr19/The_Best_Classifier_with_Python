# The_Best_Classifier_with_Python
## by Jamal Taghavimehr

## Introduction

I use two sets of data for this project. The first which is 346 records of loan data is used for the train_test split and fitting the model to the train subset of this data. This data has 8 variables among which loan_status of either paid off or defaulted is the target variable. The description of fields is as follows.

| Field          | Description                                                                           |
|----------------|---------------------------------------------------------------------------------------|
| Loan_status    | Whether a loan is paid off on in collection                                           |
| Principal      | Basic principal loan amount at the                                                    |
| Terms          | Origination terms which can be weekly (7 days), biweekly, and monthly payoff schedule |
| Effective_date | When the loan got originated and took effects                                         |
| Due_date       | Since it’s one-time payoff schedule, each loan has one single due date                |
| Age            | Age of applicant                                                                      |
| Education      | Education of applicant                                                                |
| Gender         | The gender of applicant                                                               |

For evaluation and out of sample accuracy of models I use a different dataset having the same number of fields and 54 records.
 I run 4 classification algorithms. These algorithms are KNN, Support Vector Machines, Decision Tree, and Logistic Regression.  I find the best algorithm by performing accuracy evaluation methods like jaccard index and f1 score.

## Report

| Algorithm          | Jaccard | F1-score | LogLoss |
|--------------------|---------|----------|---------|
| KNN                | 0.67    | 0.63     | NA      |
| Decision Tree      | 0.74    | 0.63     | NA      |
| SVM                | 0.74    | 0.63     | NA      |
| LogisticRegression | 0.74    | 0.63     | 0.56    |

## Conclusion

According to the evaluation matrices, all three algorithms of Decision Tree, Support Vector Machine, and Logistic Regression have the same accuracy. KNN with k=8 has the lowest accuracy compared to other machine learning algorithms.
