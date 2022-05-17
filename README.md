# Fraud-Transactions-Detection
In this project, I have used ML models to find out the transactions done by the clients are fraudulent transactions are not.

### ABOUT THE DATASET
- The dataset was provided to me by INSAID company and it consists of 6362620 rows and 11 columns.
- There was no missing values present in the dataset, when I went through the dataset,it was not balanced.
- Irrelevant or partially relevant features can have negative impact thus by using feature importance here and plotted these values just for the visualization was enough to understand what are the necessary features.
- Target variable is flagged fraud which is binary variable(0 or 1).

### Steps Followed to get the Conclusion
- The features "nameOrig" & "nameDest" are just some string values for representing the customers, which has no any significance to our data.
- The most important factors that predict fraudulent customer are initial balance recipient before the transaction and new balance recipient after the transaction.(oldbalanceDest and newbalanceDest ).
- This is a classification problem so multicolinearity won't be much of an issue, still I have implemented Decision tree and Random forest in model creation part, so as to eliminate multi-colinearity.
- I used multiple classification models like logistic regression(90%), naive bayes(74%), svm(91%), Decision tree, Random Forest. out of these model Decision tree and random forest got the highest accuracy on test data.
