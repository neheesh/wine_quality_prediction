# Wine Quality Prediction

## Project Overview
Predicting the wine quality ratings based on various features using basic machine learning models. This project was primarily focused on learning python, ML libraries, exploratory data analysis and was not intended on achieving perfect predictions.

## Dataset
- Source - [Wine Quality UCI](https://archive.ics.uci.edu/dataset/186/wine+quality) (winequality-red.csv).
- Samples - 1599 wines.
- Features - 11 physicochemical tests.
- Target - Integer rating of wine quality with a score between 3 and 8.

## Process

### Exploratory Data Analysis (EDA)
- Basic overview showing info, describe, shape, dtypes, and head.
- Plotting the distributions of target variable `quality` with majority of mediocre wines in the dataset.
- Correlation heatmap analysing between features.
- Plotting the distributions of the features like `alcohol`, `sulphates`, `citric acid`, `volatile aciditiy`.

### Preprocessing
- Splitting of data into feature and target, with `X` being features and `y` being targets.
- Splitting of data into **train** and **test** sets with 80:20 split.
- Using `StandardScaler` for avoiding training data leakage.

### Model Training and Evaluation
Training the model using regression models like,
- Linear Regression.
- Decision Tree.
- k-Nearest Neighbors.

Evaluations of the model using metrics like,
- Mean Squared Error (MSE).
- R2 Score

| Model | MSE | R2 |
|:------|:----|:---|
| Linear Regression | 0.390 | 0.403 |
| Decision Tree | 0.644 | 0.015 |
| k-NN | 0.435 | 0.335 |

### Visualization Of Results
- Plotting R2 score and MSE score in the bar charts for easy comparison.

### Conculsion
- Linear Regression with the variation ~40% performed the best.
- K-NN ~33% and decision tree regression basically the least ~1.5%.
- Visualization confirms linear regression > k-NN > Decision Tree.
- Wine quality is hard to predict with simple, default machine learning models thats being used here.
