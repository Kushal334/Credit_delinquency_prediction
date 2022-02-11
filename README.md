# Credit_delinquency_prediction

Delinquency describes something or someone who fails to accomplish that which is required by law, duty, or contractual agreement, such as the failure to make a required payment or perform a particular action.

Credit scoring algorithms, which makes a guess at the probability of default, are the method banks use to determine whether or not a loan should be granted. This use-case requires learners to improve on the state of the art in credit scoring, by predicting the probability that somebody will experience financial delinquency in the next two years.



## Data Description

The dataset consists of 150000 records and 11 features. Below are the 11 features and their descriptions.

Feature	Description :
 
SeriousDlqin2yrs - Person experienced 90 days past due delinquency or worse

RevolvingUtilizationOfUnsecuredLines - Total balance on credit cards and personal lines of credit

age - Age of borrower in years

NumberOfTime30-59DaysPastDueNotWorse - Number of times borrower has been 30-59 days past due but no worse in the last 2 years

DebtRatio - Monthly debt payments, alimony,living costs divided by monthy gross income

MonthlyIncome - Monthly Income

NumberOfOpenCreditLinesAndLoans - Number of Open loans (installment like car loan or mortgage) and Lines of credit

NumberOfTimes90DaysLate - Number of times borrower has been 90 days or more past due

NumberRealEstateLoansOrLines - Number of mortgage and real estate loans including home equity lines of credit

NumberOfTime60-89DaysPastDueNotWorse - Number of times borrower has been 60-89 days past due but no worse in the last 2 years

NumberOfDependents - Number of dependents in family excluding themselves


## Challenge
As with all the delinquency prolems, we have major class imbalance here.
92 % of customers belong to no delinquency class and 8 % for delinquency class.
We applied methods like oversampling, undersamplaing and SMOTE to tackle this problem. 

## Evaluation Metric

Recall - True Positive/True Positive + False Negative

We have selected recall as the metric here as we want to avoid False Negatives(customers who were preedicted of not default but they did).
So, we will consider recall and f1 score as our metric.
