# Datasets used in the Course

The lab exercises and tutorial in the course use several datasets. Some of these are inbuilt datasets in the scikit-learn packgae.  Others are in the data folder of this repo.  Here is a brief description of each, and a link for further information.

## MNIST Digits

The MNIST digits dataset is a collection of 70,000 hand-written digits (0-9), with 60,000 for training and 10,000 for testing. Each digit is a 28x28 pixel grayscale image.  The MNIST dataset is a well known dataset in machine learning.

It is provided as an internal dataset of the keras package.  To import it into Python, we use
> from keras.datasets import mnist

## Diabetes

The diabetes dataset has ten baseline measurements (age, sex, body mass index, average blood pressure, and six blood serum measurements) 
for 442 patients.  The label is a quantitative measure of disease progression one year after baseline measurements were taken.

The scikit learn website [here](https://scikit-learn.org/stable/datasets/toy_dataset.html#diabetes-dataset) has full details.

To import into Python, we may use:
> from sklearn import datasets
> X, y = datasets.load_diabetes(return_X_y=True)

## Telco Customer Churn

Full details on Kaggle [here](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

A copy of this data is available in the data folder of this repo

## MAGIC Gamma Telecope

This is simulated data fro a classifaction task to determine if a reading is either a gamma (signal) or a hadron (background).  There are 10 independent variables.  The source data and full details are available on the UC Irvine Machine Learning Repository [here](https://archive.ics.uci.edu/ml/datasets/magic+gamma+telescope)

A copy of this data is available in the data folder of this repo (magic04.names and magic04.data).

## Titanic

This is a partial list of some of the passengers on the Titanic.  The features are

* Survived 0 - Died, 1 - Survived
* Pclass Passenger Class
* Name   Note consistent format: \<Last name\>, \<Title\>, \<First name\> (with extra rules for married women)
* Sex
* Age
* SibSp Number of siblings (brothers/sisters)  and spouses in the party travelling with the passenger (excluding the passenger)
* Parch Number of parents and children in the party travelling with the passenger (excluding the passenger)
* Fare In GBP (1912 value)
* Embarked Point of embarkation: S - Southampton, Q - Queenstown, C - Cherbourg

## Bank Churn

This data used in [Microsoft Fabric Getting Started in Data Science Tutorial](https://learn.microsoft.com/en-us/fabric/data-science/tutorial-data-science-introduction)

There is a full description [here](https://learn.microsoft.com/en-us/fabric/data-science/tutorial-data-science-ingest-data)

The dataset contains churn status of 10,000 customers. It also includes attributes that could impact churn such as:

* Credit score
* Geographical location (Germany, France, Spain)
* Gender (male, female)
* Age
* Tenure (years of being bank's customer)
* Account balance
* Estimated salary
* Number of products that a customer has purchased through the bank
* Credit card status (whether a customer has a credit card or not)
* Active member status (whether an active bank's customer or not)

The dataset also includes columns such as row number, customer ID, and customer surname that should have no impact on customer's decision to leave the bank.

The event that defines the customer's churn is the closing of the customer's bank account. The column exited in the dataset refers to customer's abandonment. There isn't much context available about these attributes so you have to proceed without having background information about the dataset. The aim is to understand how these attributes contribute to the exited status.
