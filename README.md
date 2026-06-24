# SEO Organic Traffic Prediction using Linear Regression

## Overview

This project uses Machine Learning (Linear Regression) to predict website Organic Traffic based on key SEO metrics:

* Backlinks
* Keywords Ranked
* Page Speed Score

The project demonstrates data preprocessing, handling missing values, model training, prediction, and interpretation of regression coefficients.

## Dataset

Features (X):

* Backlinks
* Keywords Ranked
* Page Speed Score

Target Variable (y):

* Organic Traffic

Example Data:

| Organic Traffic | Backlinks | Keywords Ranked | Page Speed Score |
| --------------- | --------- | --------------- | ---------------- |
| 1200            | 50        | 100             | 70               |
| 1800            | 75        | 150             | 75               |
| 2500            | 100       | 200             | 80               |
| 3200            | NaN       | 250             | 85               |
| 4000            | 150       | 300             | 90               |

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Google Colab

## Data Preprocessing

* Removed extra spaces from column names.
* Replaced missing values in Backlinks.
* Prepared features and target variables.

## Model Training

```python
X = df[['Backlinks', 'Keywords Ranked', 'Page Speed Score']]
y = df['Organic Traffic']

lr.fit(X, y)
```

## Prediction

```python
prediction = lr.predict([[90, 180, 85]])
print(prediction)
```

## Regression Formula

Organic Traffic = Intercept + (Coefficient₁ × Backlinks) + (Coefficient₂ × Keywords Ranked) + (Coefficient₃ × Page Speed Score)

## Learning Outcomes

* Data Cleaning with Pandas
* Handling Missing Values
* Feature Selection
* Linear Regression Modeling
* SEO Data Analysis
* Making Predictions with Scikit-learn

## Author

Abdul Hye

Created as a Machine Learning practice project using SEO data and Linear Regression.
