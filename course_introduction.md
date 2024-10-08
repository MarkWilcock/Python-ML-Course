# Introduction to the Machine Learning with Python course

Welcome to the Machine Learning with Python course.  This covers "classical" machine learning - regression and classification techniques.  (We have another course on generative AI.) Classical ML uses a family of algorithm (models) to find patterns in data and use those patterns to predict useful values in new data.

Most of the course is in the form of guided tutorials and lab exercises in Python notebooks.  To do the course you need at least some basic familiarity with Python and with the numpy and pandas libraries - for example, gained in our Python foundation courses.

The course uses three Python libraries extensively;

* numpy,
* pandas and
* scikit-learn, an open-source library for supervised and upsupervised learning (explained below) with lots of tools to pre-process data, create, fit and evaluate models.

The exercises and tutorials use public datasets.  These are in the data folder of this repo.  The Datasets sections provided a brief description of each.

Dataset Terms:

* features (independent variables)
* label (target variable, dependent variable)
* training and test data
* X and y naming notation

Classical machine learning splits into two techniques

* Regression is a technique for estimating a numeric value (answering the question how much or how many)
* Classification is a technique for estimating a category. For example is an email spam or not-spam.  Is a credit card transaction fraudulent or not?  Classification can be either binary or multinomial.

Supervised and unsupervised learning are two fundamental types of machine learning.  

* In supervised learning, the model is trained using labeled data, where each input has a corresponding known output. For example, we use supervised learning to  predict house prices using historical data (features like size, location) and corresponding prices (labels).
* In unsupervised learning, the model is trained on data without labeled responses, so it tries to find hidden patterns or grouping. For example, we use unsupervised learning to group customers into different segments based on purchasing behavior

## The scikit-learn package

This is the main ML package that we use in the course.  scikit-learn offers a set of models including:

* linear regression
* logistic regression (depite its name, this is a classification model)
* SVM, a type of linear regression
* k nearest neighbours (kNN),  a model that classifies a data point based on a majority vote of its nearest neighbours
* decision trees

scikit-learn has a consistent pattern for creating and using models, regardless of the type of model being used.

1. model = a class of some Model type
2. model.fit(X, y)  
3. predictions = model.predict  

scikit-learns has several popular useful modules

* model_selection - splits data into training and test
* datasets - provides several sample datasets
* linear_model
* metrics, for measuring how good (accurate) the model is
