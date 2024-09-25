# FIFA Players Value Prediction using Machine Learning

This project predicts the market value of FIFA players using machine learning models. Various regression models are used, and their performance is evaluated using different metrics. The dataset used contains detailed information about FIFA players, including technical attributes, physical attributes, and other important data.

## Table of Contents
- Introduction
- Dataset
- Project Objective
- Data Preprocessing
- Exploratory Data Analysis
- Feature Engineering
- Modeling
- Evaluation Metrics
- Hyperparameter Tuning
- Saving and Loading the Model
- Results
- Conclusion
- Dependencies

## Introduction

This project aims to predict the market value of FIFA players based on various player attributes, such as technical skills, physical stats, and club-related data. The focus is on building and evaluating machine learning models that can accurately estimate player values.

## Dataset

- Dataset : https://data.world/raghav333/fifa-players/workspace/file?filename=fifa_cleaned.csv

The dataset used in this project is a cleaned version of the FIFA players dataset. It contains the following key attributes:

- Player's personal attributes (age, height, nationality, etc.)
- Technical skills (crossing, finishing, short passing, etc.)
- Physical attributes (stamina, strength, sprint speed, etc.)
- Club and national team information (club name, national team, wage, etc.)

## Project Objective

The objective of this project is to develop a machine learning model that accurately predicts the market value of FIFA players based on their attributes and performance metrics. The model will leverage historical data to learn patterns and relationships between player characteristics and their market value, ultimately providing a reliable tool for estimating the worth of football players in the transfer market.

## Problem Statement

In the highly competitive world of professional football, accurately assessing a player's market value is crucial for clubs, agents, and analysts. The market value of a player depends on a variety of factors, including their performance metrics, physical attributes, age, and position on the field. However, determining the correct market value can be challenging due to the complexity and interplay of these factors. An accurate prediction model would provide valuable insights, helping stakeholders make informed decisions in player transfers, contracts, and team composition.

## Data Preprocessing
Several preprocessing steps were applied to prepare the data for modeling, including:

- Removing unnecessary columns
- Handling missing values
- Handling Outliers
- Handling wrong values in columns
- Handling Multicollinearity

## Exploratory Data Analysis and Visualization

Data exploration and visualization were performed to understand the relationships between different features and the target variable (value_euro). Key findings include:

- Correlations between player attributes and market value..
- Histograms and pair plots to analyze feature distributions.

## Feature Engineering

- Encoding categorical variables (e.g., player positions)
- Scaling numerical features using MinMaxScaler
- Splitting the data into training and testing sets

## Modeling

The following machine learning models were implemented:

- 1. Random Forest Regressor
- 2. Decision Tree Regressor
- 3. Gradient Boosting Regressor
- 4. Extra Tree Regressor
- 5. Linear Regression
 
## Evaluation Metrics

The models were evaluated using the following metrics:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score

## Hyperparameter Tuning
Hyperparameter tuning was performed to optimize model performance, particularly for RandomForestRegressor, using GridSearchCV.

## Saving and Loading the Model

After training the best-performing model, it was saved for future use and predictions on unseen data.

## Results

- The Random Forest Regressor performed the best with the lowest RMSE and highest R² score.
- Linear Regression performed poorly, suggesting that a simple linear relationship is not enough to model this data

## Conclusion

The Random Forest model emerged as the best performer, showing that ensemble methods work well for predicting player values based on a variety of attributes. The model can be further improved with feature selection and hyperparameter tuning.

## Dependencies

- Python 
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn
- joblib
