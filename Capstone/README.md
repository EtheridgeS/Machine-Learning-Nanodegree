# Machine Learning Engineer Nanodegree
## Specializations
## Project: Capstone Project
## Scott Etheridge
## November 5th, 2018


## Software Requirements:
 
Python >= 3.6 
numpy >= 1.15.1
pandas >= 0.23.4
scikit-learn >= 0.20 
matplotlib >= 2.2.2
Seaborn   >= 0.9.0
Plotly  >= 0.4.0
Yellowbrick >= 0.8
imbalanced-learn >=  0.4.1
lightgbm >= 2.2.1
py-xgboost >= 0.72


## Project Overview

The Telecom industry has experienced greatly increased levels of competition over the last decade.  While the competition is coming from the traditional Telecommunications and Cable industry players, it is also coming from companies in completely different industries.  The ability to provide telecommunications service over the top (OTT) of the internet service has given companies in different industries the ability to become direct competitors.  Google and Facebook have both implemented applications and services to complete in the traditional telecom markets.  Likewise, the Wireless and Internet service markets have become commoditized services making it difficult to compete based on the quality of service/network.  

The result has been that the telecommunications companies have competed based on price.  It is never a good sign when an industry enters the stage of the product lifecycle where the only way to attract customers is based on price.  This has led to the price wars that were observed from 2015 to 2018.  Revenues have suffered greatly as a direct result of the price-based competition.  In turn, the stock price of most of the telecommunications companies has remained stagnant during this period.
I have been working in the Telecommunications industry for the last thirteen years.  I have a strong desire to help the Telecommunications companies thrive and improve their profitable - it is a matter of saving my job.  

## Problem Statement

While the Telecommunications companies are increasingly entering new markets to escape the declining wireline and wireless industries, they are also placing a laser focus on growing the revenues from their existing customer bases.  They are placing a great emphasis on reducing the number of customers that are voluntarily terminating their contracts.  The industry calls this “customer churn” – and the churn rate is defined as the percentage of the customer based that terminated their contract in the last month.  The Telecommunications industry has a churn rate of ~2% (1).  

The problem to be solved is to determine models that can be used to predict whether a customer is a candidate to terminate their contract.  The goal will be to reduce the churn rate of the standard Telecommunications Company by being able to identify customers that are likely to churn.  Then, the Telecommunications Company can target them with offers that will transform them into customers that are not likely to terminate their contract.

The problem will be set up as a classification problem.  The labeled input data contains numerical and categorical data about the customer.  Churn is the output (target) feature, which is a binary value of “Churn” or “Not Churn”.  

## Metrics

The model will be evaluated based on the model’s AUC or area under the curve associated with ROC curves.  The AUC is a common evaluation metric for binary classification problems.  Consider a plot of the true positive rate vs the false positive rate as the threshold value for classifying an item as 0 or is increased from 0 to 1: if the classifier is very good, the true positive rate will increase quickly and the area under the curve will be close to 1.  If the classifier is no better than random guessing, the true positive rate will increase linearly with the false positive rate and the area under the curve will be around 0.5.  One characteristic of the AUC is that it is independent of the fraction of the test population which is class 0 or class 1: this makes the AUC useful for evaluating the performance of classifiers on unbalanced data sets.


## Dataset

The dataset called “telco-customer-churn” will be used for this project.  (https://www.kaggle.com/blastchar/telco-customer-churn)

This dataset is from a telecommunications company and has been expressly created to support Churn analysis.  Therefore, I do believe it is relevant to this project.  Since it includes labeled variables as well as the target variable “churn”, I believe it is a good candidate for supervised machine learning algorithms.

The dataset contains 7,043 rows (customers) with 21 labeled columns.  The input data contains several continuous numerical features and several binary and multi-value categorical features about the customer.  The labeled Churn feature will be the output (target), which is a binary value of “Yes” or “No”.  

Seventy-six percent of the customers in the base dataset are “No”, while the remaining twenty-four percent of the customers are “Yes”.  
