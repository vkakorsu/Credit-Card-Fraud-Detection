# <img src="https://imgur.com/KBMMz9K.png" width="30px"> CreditCardFraud

An unsupervised learning model for detecting fraudulent credit card transactions.

## 🏦 Data

The dataset, which can be found [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), contains anonymized credit card transactions made over the course of two days in September 2013 by European cardholders.

Each transaction is labeled as fraudulent or genuine. There is a total of 285,807 transactions in the dataset, and only 492 are fraudulent. Thus, the dataset is highly unbalanced, with frauds accounting for only 0.172% of all transactions.

Due to confidentiality issues, the original features and more background information about the data is not available. As a result, features V1, V2, … V28 are the principal components obtained with PCA. The only features which have not been transformed with PCA are Time and Amount, where the Time feature contains the seconds elapsed between each transaction and the first transaction in the dataset.

The Class feature is the dependent variable and it takes value 1 in case of fraud and 0 otherwise.

## 📈 Feature Visualization

<p float="middle">
  <img align="center" src="https://imgur.com/GE9fsWA.png" width="250" />
  <img align="center" src="https://imgur.com/8oNLQm1.png" width="250" /> 
  <img align="center" src="https://imgur.com/qKFxdYM.png" width="300" />
</p>

Checking for normal distribution in all of the features ↓

<img src="https://imgur.com/qHmBCnB.png" width="400px">

## 🔍 Model Evaluation

Confusion matrix on the training set

<img src="https://imgur.com/ihwZWqv.png" width="400" />

Confusion matrix on the test set

<img src="https://imgur.com/jCI4znT.png" width="400" />

## 💡 To-do

- Use feature engineering and consider additional derived features that might be informative for detecting fraud
- Try a different unsupervised learning algorithm, such as clustering
- Use ensemble learning where the final prediction is based on the combined outputs of all models which can help reduce the impact of any one model's weaknesses
- Evaluate the model's performance using different metrics such as precision, recall, F1-score, and ROC-AUC
- Incorporate deep learning techniques
