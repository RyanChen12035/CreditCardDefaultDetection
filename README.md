# CreditCardDefault
### Description
Say we got hired by a bank in Taiwan and tried to build a model to make a prediction of whether a credit card owner will default or not based on their personal information and repayment status of six months. Throughout the EDA process, We noticed the imbalanced situation in our categorical features which may potentially cause bias so we tried to balance the dataset based on recall and precision. Also, we took log transformation on highly right-skewed numeric features to balance the data. Along with that, both types of features were applied z score normalization before feeding into the models. As for our model, we apply a fully connected network with six layers deep. We trained three models, a comprehensive one with all given features as input and able to make a prediction for next month, a more predictive one with only one month of repayment status as input so it can make a prediction 5 months ahead, and a less biased one with only repayment status and remove any potential risk of bias. In the end, we apply the ensemble technic to wrap it up and get a state-of-the-art test accuracy of 95.7% and recall of 95.4%
### Data Source
Data Contains demographic info, credit information, and history of payments and defaults of 30k credit card customers in Taiwan from April to September 2005. 
The data source is from Kaggle, UCI Machine Learning Repository
### Issue and Finding
> 1. Get to know how to deal with imbalanced data on categorical, numeric features, and label output based on the careful evaluation.
> 2. Get to know how to apply the ensemble technique to boost performance
> 3. Fully connected model training and hyperparameter tuning
## Technologies: 
Comprehensive EDA process, Feature engineering, Bias detection, Fully connected model training and hyperparameter tuning, Tensorflow data pipeline, Ensemble
## How to use this repository
W207Project1_EDA_balanced.ipynb would do the EDA process and take UCI_Credit_Card.csv which is downloaded from Kaggle as input and output a CSV file of CreditCard_EDA_balanced6636. W207project1_DataPreparation_Training_Eva_Ensemble.ipynb would then take the output CSV file as input to generate a prediction based on the models trained inside.
