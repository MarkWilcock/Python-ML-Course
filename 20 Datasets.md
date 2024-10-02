# Datasets used in the Course

The lab exercises and tutorial in the course use several datasets. Some of these are inbuilt datasets in the scikit-learn packgae.  Other are in the data folder of this repo.  Here is a brief description of each, and a link for further information.

## Bank Churn Dataset

This data used in Microsoft Fabric Getting Started in Data Science Tutorial
https://learn.microsoft.com/en-us/fabric/data-science/tutorial-data-science-introduction

Description from https://learn.microsoft.com/en-us/fabric/data-science/tutorial-data-science-ingest-data

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

## scikit-learn datasets

The inbuilt scikit-learn datasets used in the  course are:

* diabetes
* ...

<!--
to do: add these datasets if and when used.  

* kaggle: credit card fraud, email spam, house prices, cooking ingredients,...
* scikit-learn: diabetes


-->