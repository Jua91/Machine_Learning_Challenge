# Machine Learning Homework - Exoplanet Exploration

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, we will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

## Requirements

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare at least two different classifiers.

# Analysis

## Preprocessing
* In the first step, I assigned the koi_disposition as y (target) value and the rest columns as X as X (features).
* Next, I scaled and encoded the X and y values, then split them into training and testing data.

## Tuning the models

### Logistic Regression
* Training Score: , Testing Score: 
* Using GridSearchCV to tune the model's parameters and changing the grid parameters C and gamma didn't get any score improvement.

### K Nearest Neighbor

### Random Forest


### Support Vector Machine

## Model Comparison
