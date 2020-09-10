# CreditCard_FraudDetection

## General Information

* Dataset : https://www.kaggle.com/mlg-ulb/creditcardfraud
* Run in Google Collab : <a href='https://colab.research.google.com/github/chugh007/CreditCard_FraudDetection/blob/master/creditcardfraud.ipynb' target='_blank' >Credit Card Fraud</a>
* Metric Used : Area Under the ROC curve
* Technique : Anomaly Detection 

This is a classic example to practice anomaly detection . I have followed the steps from Andrew NG's machine learning tutorial for anomaly detection .

<iframe width="560" height="315" src="https://www.youtube.com/embed/086OcT-5DYI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Implementation Notes

* As mentioned in the tutorial , the features used follows gaussian distribution.
* To estimate the probability density at a point ,GaussianMixture is used .
* Training set has all non-anomolous samples
* The anomolous samples are split equally among test and validation sets.
* The optimal threshold value for highest roc_auc_score is chosen using validation set.


## Future Works

* AIC and BIC score is used to estimate the number of clusters . We can also use bayesian mixture model which can give a good estimate of the number of clusters, but it is very slow to train.








