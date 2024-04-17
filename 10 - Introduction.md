# Introduction

Welcome to the Machine Learning course.  This covers "classical" machine learning - regression and classification techniques.  (We have another course on generative AI.) Classical ML uses a family of algorithm (models) to find patterns in data and use those patterns to predict useful values in new data.

Most of the course is in the form of guided tutorials and lab exercises in Python notebooks.  To do the course you need at least some basic familiarity with Python and with the numpy and pandas libraries - for example, gained in our Python foundation and intermediate courses.

The course uses three Python libraries extensively; numpy, pandas and scikit-learn, an open-source library for supervised and upsupervised learning (explained below) with lots of tools to pre-process data, create, fit and evaluate models.

The exercise and tutorial use public datasets.  These are in the data folder of this repo.  The Datasets sections provided a brief description of each.

Dataset Terms: 
* features (independent variables)
* label (target variable, dependent variable)
* training and test data
* X and y naming notation

Classical machine learning splits into two techniques
* Regression is a technique for estimating a numeric value (answering the question how much or how many)
* Classification is a technique for estimating a category. For example is an email spam or not-spam.  Is a credit card transaction fraudulent or not?  Classification can be either binary or multinomial.


Supervised vs unsupervised learning


# scikit-learn
scikit-learn offers a set of models including 
* linear regreassion
* logistic regression (depite its name, this is a classification model)
* SVM, a type of linear regression
* k-NN,  a model that classifies a data point based on a majority vote of its nearest neighbours

scikit-learn has a consistent pattern for creating and using models, regardless of the type of model being used.
1. model = a class of some Model type
2. model.fit(X, y)  
3. predictions = model.predict  

scikit-learns has several popular useful modules
* model_selection - splits data into training and test
* datasets - provides several smaple datasets
* linear_model
* metrics, for measuring how wgood (accurate) the model is

## Course Structure

The structure of this course is 
* 10 - Introduction
* 20 - Datasets used in the Course
* 30 - Linear (least squares and SVM)  and Logistic Regression
  * Linear regression tutorial: to do
  * Linear regression lab exercise: to do
  * Logistic regression tutorial: Titanic Passenger Survival
  * Logistic regress lab exercise: to do (use bank churn)  
* 40 - Other Classification Models: k Nearest neighbours (kNN), Naive Bayes,  Lab to comapre and evaluate several models
  * Tutorial for each
  * Lab exercise for each
* 50 - Unsupervised techniques.  Clustering
* 70 * Deep learning. Building neural nets.  keras, tensorflow and PyTorch packages (optional advanced section)
* 90 - Resources


