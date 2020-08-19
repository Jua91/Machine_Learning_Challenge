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

## Analysis

### Preprocessing
* In the first step, I assigned the `koi_disposition` as y (target) value and the rest columns as X (features).
* Next, I scaled and encoded the X and y values, then split them into training and testing data.

### Tuning the models
* Using `GridSearchCV` to tune the model's parameters and changing the grid parameters

## Model Comparison

### Models

#### Logistic Regression
* Training Data Score: `0.851`, Testing Data Score: `0.843`
* Best Score after Hyperparameter Tuning: `0.878`

#### K Nearest Neighbor
* Training Data Score: `0.882`, Testing Data Score: `0.837`
* Best Score after Hyperparameter Tuning: `0.840` (where `k=7`)

#### Random Forest
* Training Data Score: `1.0`, Testing Data Score: `0.890`
* Best Score after Hyperparameter Tuning: `0.892`

#### Support Vector Machine
* Training Data Score: `0.845`, Testing Data Score: `0.833`
* Best Score after Hyperparameter Tuning: `0.881`

### Model Selection
Comparing all four models, the random forest yielded the highest score after hypterparameters tuning. Therefore, the random forest model is better than the other three models.
