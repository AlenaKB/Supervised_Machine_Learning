# Credit Risk Analysis

## Project Objective: 
Use imbalanced-learn and scikit-learn libraries to build and evaluate models, and make a recommendation on whether they should be used to predict credit risk. The main objective is to address the class imbalance and the ways it can be solved, since binary classification is becoming such a popular application for supervised machine learning. By applyng several oversampling techniques and ensemble learners, I tried to solve this problem.

### Methods Used:
- Machine Learning
- Predictive Modeling
- Descriptive and Inferential Statistics 

### Technologies: 
- Python 3.0
- scikit-learn library
- imbalanced-learn library 

## Project Description 

1. credit_risk_resampling
I explored 5 different methods for dealing with imbalanced datasets:
I used several different resampling techniques: RandomOverSampler and SMOTE algorithms, tried the cluster centroid, and 
the SMOTEENN algorithms. 

To begin with, all models came up with extremely low precision in predicting high risk loans, 0.01. Which tells us, there are lots of false positives. 
And we see an incredible 100% precision in detecting low risk applications. I can conclude none of the models did a great job. Especially, if we look at the accuracy scores, the highest score being 64 and the lowest - 54. 

However, the random oversampling method showed a pretty decent recall rate - 70% in predicting high risk applicants. And undersampling being the most ineffective - 48. 

Maybe, resampling shouldn't be the stand alone solution, and rather coupled with additional methods. Like, rebalnce in a different proportion, or getting additional features to enrich the dataset. 

2. credit_risk_ensemble

The ensemble models performance is much better than the latter ones. Even though, AdaBoost showed a pretty low precision in identifying high risk applications, it showed a nice recall rate. Which tells us high risk is well detected but there is also 
some amount of false negatives. Plus, the AdaBoost's accuracy score is great, 0.90. 

Balanced Random Forest managed to get quite a low accuracy score, compared to AdaBoost - 0.67. Its precision rate is very high, the recall rate of finding high risks being signifcantly lower - 0.35. Which says the model fails at detecting the class well. Has perfect metrics in classyfying the low risk applications, 100% in both precision and sensitivity. 

Between two models, I would definitely use AdaBoost, because in the case of detecting such things as high risk applicants, we can sacrifice precision, but rather have higher sensitivity, and AB is doing a pretty good job in finding those. 





