# home-credit-kaggle-competition
The Home credit default risk machine learning competition's main objective was to predict whether or not the applicant will be able to repay the loan which is a standard supervised classification task:

<b>Supervised</b>: The labels are included in the training data and the goal is to train a model to learn to predict the labels from the features

<b>Classification</b>: The label is a binary variable, 0 (will repay loan on time), 1 (will have difficulty repaying loan)

The data comprised of 7 different files:

<b>application_train/application_test</b>: the main training and testing data with information about each loan application at Home Credit. Every loan has its own row and is identified by the feature SK_ID_CURR. The training application data comes with the TARGET indicating 0: the loan was repaid or 1: the loan was not repaid.

<b>bureau</b>: data concerning client's previous credits from other financial institutions. Each previous credit has its own row in bureau, but one loan in the application data can have multiple previous credits.

<b>bureau_balance</b>: monthly data about the previous credits in bureau. Each row is one month of a previous credit, and a single previous credit can have multiple rows, one for each month of the credit length.

<b>previous_application</b>: previous applications for loans at Home Credit of clients who have loans in the application data. Each current loan in the application data can have multiple previous loans. Each previous application has one row and is identified by the feature SK_ID_PREV.

<b>POS_CASH_BALANCE</b>: monthly data about previous point of sale or cash loans clients have had with Home Credit. Each row is one month of a previous point of sale or cash loan, and a single previous loan can have many rows.

<b>credit_card_balance</b>: monthly data about previous credit cards clients have had with Home Credit. Each row is one month of a credit card balance, and a single credit card can have many rows.

<b>installments_payment</b>: payment history for previous loans at Home Credit. There is one row for every made payment and one row for every missed payment.


The diagram shows how the data is related:
![home_credit_overview](https://user-images.githubusercontent.com/25699909/44066384-a75d01cc-9f35-11e8-84a8-fe60cbeedfcf.PNG)

This is an online machine learning competition, currently being hosted on kaggle website. The files in this repository provide insights to 
Exploratory Data Analysis and achieves an accuracy of 79.2% with the basic first level machine learning model 
(using Microsoft's LightGBM library).

This project is in progress and currently, we are engineering the features to improve the current ML model.  

# Credits 
Will Koehrsen (https://www.kaggle.com/willkoehrsen)

Olivier (https://www.kaggle.com/ogrellier)

Aguiar (https://www.kaggle.com/jsaguiar)
