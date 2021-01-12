# Parul_Portfolio
Data Science Projects

[Project1:German Credit Risk Project ](https://github.com/ps1608/ps_2019/edit/master/XlriExitProject_GermanCreditRisk)

•	German Credit Risk data from Kaggle for XLRI exit project

•	As per project requirement, analyzed financial inputs to calculate baseline misclassification Loss to come up with Business Justification Plan

•	Feature Engineered data to create Flags for LowBalance Accounts and quantified EMI 

•	Optimized Random Forest, Logistic Regression & Decision Tree using CV 

•	Took the probability of default from Model , to build a Credit Risk Dashboard for computation of Key Business Metrics (i.e Expected Loss) and classified customers into Highly Risk,Risky & Less Risky categories.

[Credit Risk Dashboard](https://public.tableau.com/profile/psald2415#!/vizhome/GermanCreditRisk_Dashboard/CreditRiskDashboard)

![](/images/RiskvsCredit.png)

![](/images/LogisticRegressionCostFunction.png)



[Project2:Demand Forecasting](https://github.com/ps1608/ps_2019/tree/master/DemandForecast)

The problem is of a retail chain which wants to use it is 3 years past data(130 weeks data)
demand/units _sold for 28 products(sku’s) across 76 stores, to predict/forecast the demand for next 
12 weeks accurately. However, since we do not have Actual demand data for test set . the first 120.The data is captured at the beginning of each week

•	This is a multiple time series , with other inputs like flags whether it’s a featured sku/on display sku ,base price an totalpriceetc besides starting Dateof week

•	Did Exploratory analysis for couple of time series and they had seasonality effect

•	Feature Engineered  to quantify Price ration (total price/base price)

•	Featured Engineered to extract month information from week

•	Tried models like auto.arima with xreg & xgboost  xgbosst performed better.

•	Optimized xgboost  with CVgridSearch                  

![](/images/dfcor.png)


[Project 3: Fraud Detection Project](https://github.com/ps1608/ps_2019/tree/master/Fraud%20Detection)

It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.
The datasets contains transactions made by credit cards in September 2013 by european cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

. Given the Imbalance AUCPR is the identified Metric

. Due to Confidentiality Issues, Features are Principal Components obtained with PCA

. 'Melt' used to plot boxplot for different features ,for Outlier identification and Outliers removed

. Tried weighted Logistic Regression / Cart . Though both models gave decent AUCPR ,with all featureds

. Used FeaturePlot & Backward Elimination to identify important features.

. Finally CART selected as it easy to interpret and gives 0.70 AUCPR on train set and 0.69 AUCPR on test set




