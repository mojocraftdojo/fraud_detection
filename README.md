# Modeling for Credit Card Fraud Detection

The Credit Card Fraud Detection Problem includes modeling the past credit card transactions with known fraud transactions. 

The goal for this project is to predict fraudulent transactions while minimizing the incorrect fraud classifications.

The dataset contains more than 284k transactions and 30 features which most of them have already been PCA transformed, but there are still EDA work need to be done before modeling.
For example, Data cleaning, transformation and feature selection. Majority of transactions are non fraud, thus this is a highly imbalanced dataset. 

The machine learning models tested and compared here are: 

   -- Logistic Regression
   
   -- Support Vector Machine
   
   -- Random Forest
   
   -- XGBoost
   
   -- CatBoost
   
   -- Gradient Boosting

The above models are built using scikit-learn framework

Other than these, an Artificial Neural Network (ANNs) model is also trained to compare with the above ML models. The ANN model is built using Keras/Tensorflow 2.0 framework. 
