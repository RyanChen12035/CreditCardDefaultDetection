# CreditCardDefault
### Description
Say we got hired by a bank in Taiwan and tried to build a model to make a prediction of whether a credit card owner will default or not based on their personal information and repayment status. Throughout the EDA process, We noticed the imbalanced situation in our categorical features which may potentially cause bias so we tried to balance the dataset based on recall and precision. Also, we took log transformation on highly right-skewed numeric features to balance the data. Along with that, both types of features were applied z score normalization before feeding into the models. As for our model, we apply a fully connected network with six layers deep. We trained three models, a comprehensive one with all given features as input and able to make a prediction for next month, a more predictive one with only one month of repayment status as input so it can make a prediction 5 months ahead, and a less biased one with only repayment status and remove any potential risk of bias. In the end, we apply the ensemble technic to wrap it up and get a state-of-the-art test accuracy of 95.7% and recall of 95.4%
### Data Source
Data Contains demographic info, credit information, and history of payments and defaults of 30k credit card customers in Taiwan from April to September 2005. 
The data source is from Kaggle, UCI Machine Learning Repository
### Issue and Finding
1. Learn how to deal with imbalanced data on categorical, numeric features, and label output based on strictly evaluating.
2. Learn how to apply the ensemble technique to boost performance
### Technologies: 
Comprehensive EDA process, Feature engineering, Bias detection, tunning of Fully connected Model, Tensorflow data pipeline, Ensemble
