# Datasets used in the Course

The lab exercises and tutorial in the course use several datasets. Some of these are inbuilt datasets in the scikit-learn package.  Others are in the data folder of this repo.  Here is a brief description of each, and a link for further information.

## Titanic

This is a partial list of some of the passengers on the Titanic.  [Full details are available on this page](https://zomalex.co.uk/datasets/titanic_dataset.html)

## Bank Churn

This fictional  dataset contains churn status of 10,000 bank customers.  Full details are available on [this page](https://zomalex.co.uk/datasets/bank_churn_dataset.html)

## MNIST Digits

The MNIST digits dataset is a collection of 70,000 hand-written digits (0-9), with 60,000 for training and 10,000 for testing. Each digit is a 28x28 pixel grayscale image.  The MNIST dataset is a well known dataset in machine learning.

It is provided as an internal dataset of the keras package.  To import it into Python, we use
> from keras.datasets import mnist

## Diabetes

The diabetes dataset has ten baseline measurements (age, sex, body mass index, average blood pressure, and six blood serum measurements) for 442 patients.  The label is a quantitative measure of disease progression one year after baseline measurements were taken.

The [scikit learn website](https://scikit-learn.org/stable/datasets/toy_dataset.html#diabetes-dataset) has full details.

To import into Python, we may use:
> from sklearn import datasets  
> X, y = datasets.load_diabetes(return_X_y=True)

## Telco Customer Churn

Full details on Kaggle [here](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

A copy of this data is available in the data folder of this repo [here](./data/telco_customer_churn.csv)

## MAGIC Gamma Telescope

This is simulated data for a classification task to determine if a reading is either a gamma (signal) or a hadron (background).  There are 10 independent variables.  The source data and full details are available on the [UC Irvine Machine Learning Repository here](https://archive.ics.uci.edu/ml/datasets/magic+gamma+telescope)

A copy of this data is available in the data folder of this repo.

* [magic04.data](data/magic04.data) is the data file
* [magic04.names](data/magic04.names) is the description file
