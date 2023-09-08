# Modeling for Credit Card Fraud Detection

The Credit Card Fraud Detection Problem includes modeling the past credit card transactions with known fraud transactions. 

The goal for this project is to predict fraudulent transactions while minimizing the incorrect fraud classifications.

The dataset contains more than 284k transactions and 30 features which most of them have already been PCA transformed, but there are still EDA work need to be done before modeling.
For example, Data cleaning, transformation and feature selection. Majority of transactions are not fraudulent, thus making this dataset highly imbalanced.

The machine learning models tested and compared here are: 

   -- Logistic Regression (Baseline)
   
   -- Support Vector Machine
   
   -- Random Forest
   
   -- XGBoost
   
   -- CatBoost
   
   -- Gradient Boosting

The above models are built using scikit-learn framework. Logistic Regression is used as a baseline that all other models will be compared to. 

Other than these, an Artificial Neural Network (ANNs) model is also trained to compare with the above ML models. The ANN model is built using Keras/Tensorflow 2.0 framework. 




### **Highlighted results:**

---  All models perform better on training set than testing set, which is expected

---  Based on F1-score , the top performing classifiers for this dataset are CatBoost, Random Forest , XGBoost and ANNs(see below figure). These models all easily pass F1 score cutoff (F1>=0.8). ANNs's performance seems slightly lower than the other three, but there is room for improvement given more epoch runs and hyperparameter turning.

---  CatBoost, Random Forest and XGBoost are trained using out-of-box parameters without any tuning, they all can achieve F1 score in 0.8 ~ 0.9 range.

---  Logistic Regression, Gradient Boost and SVM achieved F1 score in 0.7 ~ 0.8 range. Classification threshold adjustment has been attempted to boost performance when running Logistic Regression. 

![F1-scores](https://github.com/mojocraftdojo/fraud_detection/blob/main/model_performance_comparison.png "Model Comparison")

