# Introduction to the Machine Learning with Python course

Welcome to the Machine Learning with Python course. This course covers "classical" machine learning: regression and classification techniques. (We have another course on generative AI.) Classical ML uses a family of algorithms (models) to find patterns in data and use those patterns to predict useful values in new data.

Most of the course is in the form of guided tutorials and lab exercises in Python notebooks. To do the course you need at least some basic familiarity with Python and with the numpy and pandas libraries - for example, gained in our Python foundation and intermediate courses.

The course uses three Python libraries extensively:

* numpy
* pandas
* scikit-learn, an open-source library for supervised and unsupervised learning (explained below) with lots of tools to pre-process data, create, fit and evaluate models.

The exercises and tutorials use public datasets. The Datasets page provides a brief description of each and links to more details.

## Dataset Terms

In machine learning we use these terms to describe datasets:

* features (independent variables)
* label (target variable, dependent variable)
* X and y naming notation

## Types of Variables

A variable can either be numeric (continuous or discrete) or categorical (a set of categories or classes).

Numeric values can be discrete (e.g. counts like number of children) or continuous (e.g. measurements like height, weight, temperature).

Categorical variables indicate distinct groups or categories. For example,

* journey type (e.g. business, leisure)
* crime category (e.g. burglary, robbery, fraud)
* product category (e.g. electronics, clothing, furniture)

Nominal variables are categorical variables with no inherent order. The values are labels only, and their order does not matter, for example:

* types of fruits: apples, bananas, oranges
* car makes: VW, BMW, Audi
* countries in the United Kingdom (England, Scotland, Wales, Northern Ireland)

Ordinal variables are categorical variables that do have a natural order. The values reflect ranking or progression, though the exact differences between levels may not be measurable. For example:

* education levels: GCSE -> A-level -> university degree
* body mass index (BMI) classification: underweight -> normal -> overweight -> obese
* customer satisfaction: poor -> fair -> good -> excellent
* days of the week (Monday -> Sunday) or months of the year (January -> December) (Although days and months are technically cyclical, we usually treat them as ordered categories.)

## ML terms and techniques

Classical machine learning splits into two techniques:

* Regression is a technique for estimating a numeric value (answering the question how much or how many).
* Classification is a technique for estimating a category. For example, is an email spam or not-spam? Is a credit card transaction fraudulent or not? Classification can be either binary (A or B) or multinomial (A or B or C or ...).

Supervised and unsupervised learning are two fundamental types of machine learning.

* In supervised learning, the model is trained using labeled data, where each input has a corresponding known output. For example, we use supervised learning to predict house prices using historical data (features like size, location) and corresponding prices (labels).
* In unsupervised learning, the model is trained on data without labeled responses, so it tries to find hidden patterns or grouping. For example, we use unsupervised learning to group customers into different segments based on purchasing behavior.

To evaluate a model, we typically split the dataset into training and test sets. The model is trained on the training set and then evaluated on the test set to see how well it generalizes to new, unseen data. Typically we may use 70% of the data for training and 30% for testing, or a 70/30 split, but this can vary depending on the dataset size and complexity.

The machine learning workflow typically involves the following steps:

1. Split a dataset into training and test sets.
1. Train a chosen algorithm with the training data -> model.
1. Test that model works well by evaluating it with the test data -> accuracy.
1. Use model + new data to make predictions.

## The scikit-learn package

This is the main ML package that we use in the course. scikit-learn offers a set of models including:

* linear regression
* logistic regression (despite its name, this is a classification model)
* k nearest neighbours (kNN), a model that classifies a data point based on a majority vote of its nearest neighbours
* decision trees
* support vector machines (SVM), which can be used for classification (SVC) and regression (SVR)

scikit-learn has a consistent pattern for creating and using models, regardless of the type of model being used.

```python
model = SomeModelClass()
model.fit(X, y)
predictions = model.predict(X_test)
```

scikit-learn has several popular useful modules:

* model_selection - splits data into training and test
* datasets - provides several sample datasets
* linear_model
* metrics, for measuring how good (accurate) the model is
