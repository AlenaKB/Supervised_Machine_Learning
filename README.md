# supervised_ml
## credit risk analysis

1. credit_risk_resampling
I explored 5 different methods for dealing with imbalanced datasets:
I used several different resampling techniques: RandomOverSampler and SMOTE algorithms, tried the cluster centroid, and 
the SMOTEENN algorithms. 

To begin with, all models came up with extremely low precision in predicting high risk loans, 0.01. Which tells us, there are lots of false positives. 
And we see an incredible 100% precision in detecting low risk applications. I can conclude none of the models did a great job. Especially, if we look at the accuracy scores, the highest score being 64 and the lowest - 54. 

However, the random oversampling method showed a pretty decent recall rate - 70% in predicting high risk applicants. And undersampling being the most ineffective - 48. 

Maybe, resampling shouldn't be the stand alone solution, and rather coupled with additional methods. Like, rabalnce in a different proportion, or getting additional features to enrich the dataset. 

2. credit_risk_ensemble

The ensemble models performance is much better than the latter ones. Even though, AdaBoost showed a pretty low precision in identifying high risk applications, it showed a nice recall rate. Which tells us high risk is well detected but there is also 
some amount of false negatives. Plus, the AdaBoost's accuracy score is great, 0.90. 
Balanced Random Forest not showing as imoressive result, 0.67 score. However, its precision rate is very high, the recall rate of finding high risks being signifcantly lower - 0.35. Which says the model fails at detecting the class well. 

Between two models, I would definitely use AdaBoost, because in the case of detecting such things as high risk applicants, we can sucrifice precision, but rather have higher sensitivity. 





