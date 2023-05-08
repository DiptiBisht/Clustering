# Clustering
(1) Use of a clustering method (unsupervised learning),

(2) Hyperparameter tuning (manually) in clustering,

(3) Using a clustering method to characterize a phenomenon and provide insights.

(4) Do classification using a clustering method

Problem 1 - Credit Card Dataset for Clustering

This is a Kaggle dataset and is available at: Credit Card Dataset for Clustering | Kaggle (Links to an external site.) 

Abstract

This case requires one to develop a customer segmentation model to define a marketing strategy. The sample dataset summarizes the usage behavior of about 9000 active credit card holders during the last 6 months. The file is at a customer level with 18 behavioral variables.

Following is the Data Dictionary for Credit Card dataset :-

CUSTID : Identification of Credit Card holder (Categorical)
BALANCE : Balance amount left in their account to make purchases (
BALANCEFREQUENCY : How frequently the Balance is updated, score between 0 and 1 (1 = frequently updated, 0 = not frequently updated)
PURCHASES : Amount of purchases made from account
ONEOFFPURCHASES : Maximum purchase amount done in one-go
INSTALLMENTSPURCHASES : Amount of purchase done in installment
CASHADVANCE : Cash advance given to the user
PURCHASESFREQUENCY : How frequently the Purchases are being made, score between 0 and 1 (1 = frequently purchased, 0 = not frequently purchased)
ONEOFFPURCHASESFREQUENCY : How frequently Purchases are happening in one-go (1 = frequently purchased, 0 = not frequently purchased)
PURCHASESINSTALLMENTSFREQUENCY : How frequently purchases in installments are being done (1 = frequently done, 0 = not frequently done)
CASHADVANCEFREQUENCY : How frequently the cash in advance being paid
CASHADVANCETRX : Number of Transactions made with "Cash in Advanced"
PURCHASESTRX : Number of purchase transactions made
CREDITLIMIT : Limit of Credit Card for user
PAYMENTS : Amount of Payment done by user
MINIMUM_PAYMENTS : Minimum amount of payments made by user
PRCFULLPAYMENT : Percent of full payment paid by user
TENURE : Tenure of credit card service for user

To Do:

(1) For this problem, characterize customers who

     (a) make frequent purchases using the credit card. The variable PURCHASESFREQUENCY could be an

          indicator of frequency of usage.

     (b) have high balances in their account. The variable BALANCE could be used for this characterization.

(2) Try manual tuning of hyperparameters to get the best set of clusters to characterize each phenomenon.

=========================================================

Problem 2- South German Credit Data

The problem description, data and other details are available at:

https://archive.ics.uci.edu/ml/datasets/South+German+Credit+%28UPDATE%29 (Links to an external site.) 

A more extensive discussion of the problem is available in this paper:

http://www1.beuth-hochschule.de/FB_II/reports/Report-2019-004.pdf (Links to an external site.) 

Background Information

Häußler (1979, 1981) and Fahrmeir and Hamerle (1981, 1984) gave an account on the story behind the data, which is summarized here: the data are a stratified sample of 1000 credits (300 bad ones and 700 good ones) from the years 1973 to 1975 from a large regional bank in southern Germany, which had about 500 branches, among them both urban and rural ones. Bad credits are heavily oversampled, in order to acquire sufficient information for discriminating them from good ones; the sources report that the actual prevalence of bad credits is around 5%; thus, in a Bayesian context, 5% might be used as a prior probability for a credit being bad. As suggested with the Statlog German credit data, one might consider misclassification cost, and it has been suggested to allocate the cost for misclassifying a bad risk as good to be five times as high than the cost for misclassifying a good risk as bad. The credits are part of normal bank business, i.e. all debtors must have passed some checks of creditworthiness before being granted the credit; this, of course poses a severe limitation for the usability of the data in support of credit decisions for general requests (as was also noted e.g. by Häußler 1979). According to Fahrmeir and Hamerle (1984), customers with “good” credits perfectly complied with the conditions of the contract while customers with “bad” credits did not comply with the contract as required.

 

To Do:

(1) This is a classification problem, but you will instead use the dataset to find groupings through clustering. Try to group debtors using K-means clustering so that there are distinct groups corresponding to those who are "bad" credits vs those who are "good." DO NOT USE THE TARGET COLUMN "Kredit" WHEN DOING CLUSTERING. But, use the target values after clustering and compute the percentage of good credit ("1" in the target column) vs bad credit ("0" in the target column) for each group and your overall accuracy of prediction using clustering.

(2) Try manual tuning of hyperparameters to get the best set of clusters.

(3) Using appropriate features, explain/characterize debtors who are bad credits ("0" in the Target column).

NOTE: You can open the ASC data file in Excel. But here's a copy since some could not unzip the file.
