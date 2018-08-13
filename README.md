# Credit-Card-Fraud-Detection-Autoencoder
Using Autoencoder to detect credit card fraud demo source : https://www.kaggle.com/pgladkov/fraud-detection-using-autoencoder


## Using Auto Encoders for Anomaly Detection
The idea to apply it to anomaly detection is very straightforward:

i) train an auto-encoder on X_train with good regularization

ii) evaluate it on the validation set X_val and visualise the reconstructed error plot

iii) choose a threshold which determines whether a value is an outlier (anomalies) or not

## Data set
The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

**link source:**  https://www.kaggle.com/pgladkov/fraud-detection-using-autoencoder/data  
