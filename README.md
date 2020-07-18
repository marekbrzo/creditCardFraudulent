# creditCardFraudulent
Machine Learning Algorithms to Predict Fraudulent Claims

# Proposal

## Abstract
Credit card companies are actively trying to recognize fraudulent credit card transactions to prevent customer grief for the charges they have not purchased. I predict applying machine learning techniques on credit card transactional data can help prevent fraudulent purchases. To test this hypothesis, data will be imported from a public, non-affiliated credit card company dataset, off Kaggle. Finally, support vector machine ML algorithms will be applied.

## Introduction
In the modern world, purchasers are increasingly using their credit cards [1]. Americans currently use Visa-branded and Mastercard-branded credit cards more than 33 billion times per year [2]. Additionally, over 70% of purchasers claim they own credit cards [3]. Credit card fraud cost users and banks billions of dollars per year [4].

## Dataset
As mentioned, the dataset that will be explored contains transactions made by credit cards by European cardholders for the month of September 2013. The dataset encompasses credit transactions that occurred in two days. Of the entire 284,807 transactions 492 are frauds. This dataset is quite unbalanced with an actual true fraud case accounting for 0.172% of all transactions.
The dataset is in a clean csv file, found on Kaggle. The data only contains numerical input variables which are a result of a PCA transformation [5]. The data lacks complete information, because of data masking, due to data security (personal confidentiality). The only features that have not been transformed with  PCA are ‘Time’ and ‘Amount.’  Feature ‘Time’ contains the seconds elapsed between each transaction and the first transaction in the dataset. While Feature ‘Amount’ is the transaction amount. Lastly, the predicting feature ‘Class’ is the response variable and it takes a value of 1 for fraud and 0 otherwise.

## Methods
Various machine learning (ML) methods will be implemented to help predict credit card fraud. The model that will be constructed will be focused primarily looking for correlations, as well as any patterns between the features. While this model is descriptive and retro-looking, it can be effectively remodeled to be a forward-looking predictive model. Again, the project will be using one public dataset, which will be profiled, cleansed and prepared for supervised and unsupervised ML algorithms.
	From BDA104, ML methods that have been discussed will be implemented onto this dataset: Linear & Multivariate Regression, Logistic Regression, Decision Tree. In addition, Random Forest with various boosters such as XGBoost and AdaBoostClassifer  and K-Nearest Neighbour will also be exercised on the dataset. One ML method I am excited to implement is Support Vector Machines (SVM). Since we do not fully cover all methods in class, it will be interesting to see how these last three methods might compare to others. 
Recommendation given from Kaggle: Due to the class imbalance ratio, measuring accuracy using the Area Under the Precision-Recall Curve (AUPRC).

## Reference
[1] Steele, J., Johnson, A., Credit card use and availability statistics, January 2020, Creditcards.com, https://www.creditcards.com/credit-card-news/credit-card-use-availability-statistics-1276/, Research and Statistics, July 2020

[2] Mckinley, R., How Many Card Purchases do Americans Make on Credit Cards and Debit Cards, March 2019, CardTrak.com  https://cardtrak.com/2019/03/14/spending/how-many-card-purchases-on-do-americans-make-on-credit-cards-and-debit-cards/#:~:text=Americans%20currently%20use%20Visa-branded%20and%20Mastercard-branded%20credit%2Fcharge%20cards,made%20annually%20on%20Visa-branded%20and%20Mastercard-branded%20debit%2Fprepaid%20cards., July 2020

[3] Board of Governors of the Federal Reserve System, May 2017, Federal Reserve, https://www.federalreserve.gov/publications/files/2016-report-economic-well-being-us-households-201705.pdf,July 2020

[4] Credit Card Fraud Statistics, July 2020, Shift https://shiftprocessing.com/credit-card-fraud-statistics/ , July 2020

[5] Machine Learning Group – ULB, Anonymized credit card transactions labeled as fraudulent or genuine, 2018, Kaggle https://www.kaggle.com/mlg-ulb/creditcardfraud ,July 2020 (DATASET)
