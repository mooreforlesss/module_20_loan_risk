# Module 12 Report Template

## Overview of the Analysis

The purpose of this anaylsis is to see which models would best determine wether a loan is healthy or high-risk based on certain parameters given. It's important to know wether or not a loan is healthy or not so that the company that issued the loan can know wether or not the person or entity that took out the loan will pay it back or not. The parameters the model used was the size of the loan, interest rate, income of the borrower, debt to income of the borrower, number of accounts the borrower has, any sort of derogatory marks, and total debt. An issue with using this data is that almost 97% of the loans are healhty loans, so it's difficult to determine unhealhty loans when there is only a little over 3% of the data with unhealhty loans. I used a number of different models to determine which model would turn out the best. I started with a logistic regression model that turned out great, but wanted to continue to see if there were any other models that could perform better. I used the random forest classifier, K Neighbors classifier, Ada boost classifier, and gradient boosting classifier to test out a number of different types of models.


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Logistic Regression:
    * The logistic regression had one of the better results with a precision score of 1, recall of 0.99, and a f1 of 1 when determining healthy loans. It had a precision score of 0.85, a recall of 0.98 and a f1 of 0.91 when determing a unhealthy loan.
* Random Forest Classifier:
    * The Random Forest Classifier had the worst results with a precision score of 1, recall of 1, and a f1 of 1 when determining healthy loans; however, it also had a precision score of 0.88, a recall of 0.87 and a f1 of 0.87 when determing a unhealthy loan.
* K Neighbors Classifier:
    * The K Neighbors Classifier had a great result with a precision score of 1, recall of 1, and a f1 of 1 when determining healthy loans. It had a precision score of 0.87, a recall of 0.99 and a f1 of 0.93 when determing a unhealthy loan.
* Ada Boost Classifier:
    * The Ada Boost Classifier also had one of the better results with a precision score of 1, recall of 1, and a f1 of 1 when determining healthy loans. It had a precision score of 0.87, a recall of 0.99 and a f1 of 0.93 when determing a unhealthy loan.
* Gradient Boosting Classifier:
    * The Gradient Boosting Classifier also had one of the better results with a precision score of 1, recall of 1, and a f1 of 1 when determining healthy loans. It had a precision score of 0.87, a recall of 0.99 and a f1 of 0.93 when determing a unhealthy loan. However it had 1 more false negative and false positive compared to Ada Boost Classifier.

## Summary

In summary these models as a whole did really well all together, but there are a few that are better than the rest. The two best models would be AdaBoostClassifier and GradientBoostingClassifer with AdaBoost beating it out by just 1 false negative and false positive. In this scenario you want the least amount of false negatives because you don't want a predicted healhty loan to turn out to be a unhelahty loan. It's much better for a predicted unhealhty loan to turn out to be a healhty loan. It is clear that these are the two best models because they have the best precision and recall score than the reest of the models. 
