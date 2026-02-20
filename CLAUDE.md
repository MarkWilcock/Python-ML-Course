# CLAUDE.md

## Project Overview

This is a **Machine Learning with Python** course repository. It contains Jupyter notebooks teaching scikit-learn and Keras for regression, classification, and deep learning tasks.

## Notebooks

| Notebook | Topic | Dataset |
|---|---|---|
| `regression_mtcars.ipynb` | Linear Regression (intro) | MTCars |
| `linear_regression_diabetes.ipynb` | Linear Regression (scikit-learn) | Diabetes |
| `classification_bank_churn.ipynb` | Classification (intro) | Bank Churn |
| `classification_titanic.ipynb` | Classification (scikit-learn) | Titanic |
| `svc_digits.ipynb` | Support Vector Classifier | MNIST Digits |
| `keras_mnist.ipynb` | Neural Net / Deep Learning | MNIST Digits |
| `keras_telco_churn.ipynb` | Neural Net / Deep Learning | Telco Churn |
| `telescope.ipynb` | KNN & Naive Bayes (hidden) | MAGIC Gamma Telescope |

## Running Tests

Notebooks are smoke-tested using [nbmake](https://github.com/treebeardtech/nbmake):

```bash
pytest
```

Configuration is in `pytest.ini`. The timeout is set to 600s per notebook to accommodate Keras training time.

## Key Libraries

- **scikit-learn** — regression, classification, SVC
- **Keras / TensorFlow** — neural networks
- **pandas, numpy** — data manipulation
- **matplotlib** — visualisation

## Data

- Built-in datasets (scikit-learn, Keras): Diabetes, MNIST Digits
- CSV files in `data/`: Telco Churn, MAGIC Gamma Telescope, MTCars, Bank Churn, Titanic
