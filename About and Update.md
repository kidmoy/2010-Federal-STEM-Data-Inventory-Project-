# 2010-Federal-STEM-Data-Inventory-Project-Log

First I took the the target variable creators into the modeling procedure and went forward to fit a regularised logistic regression to get a lift in the AUC of ROC_AUC: 0.7348 without any regularization and a lift of ROC_AUC: 0.7993 after tuning of the hyperparameters.
(Please refer to the Intial Trails notebook)

We have to keep in mind that only a bare bone Logistic Regression model using only the numerical funding variables gave us a lift of ROC_AUC: 0.8548.
Hence the near perfectly correlated creator variables of FY2008, FY2009 were adding a creator bias to the model and adding more feature variables was just adding noise to the already established relation. So I decided to drop the creator variables and proceed with the modeling and till now have got a max lift ROC_AUC: 0.5996 with the tuned XGBoost model. (Please refer to the Submission notebook) 
