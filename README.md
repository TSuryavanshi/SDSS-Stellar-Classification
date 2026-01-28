# Predicting Stars, Galaxies & Quasars with ML

This repository contains a machine learning workflow designed to classify celestial objects into three categories: 
- Stars
- Galaxies
- Quasars

By analyzing photometric data and spectroscopic redshift, the models aim to automate the identification process for large-scale astronomical surveys.

## Overview
The project processes data from the SDSS "Skyserver" dataset. 
It involves exploratory data analysis (EDA), data cleaning (dropping unique identifiers like objid), and feature engineering. 
The core of the project is the comparison of multiple classification models to determine the most effective approach for astronomical classification.

## DatasetThe dataset consists of 10,000 observations with 18 features:
- Photometric Filters: $u, g, r, i, z$ (magnitudes across different wavelengths).
- Spectroscopic Features: redshift (crucial for distinguishing between stars and distant galaxies/quasars).
- Positional Data: ra (Right Ascension) and dec (Declination).
- Target Class: Star, Galaxy, or Quasar.

## Tech Stack
Language: Python
Libraries:
- Data Handling: pandas, numpy
- Visualization: matplotlib, seaborn
- Machine Learning: scikit-learn, tensorflow/keras

## Machine Learning Models
The notebook implements and compares the following models:
- Logistic Regression: A baseline linear classifier.
- Decision Tree Classifier: Captures non-linear relationships.
- K-Nearest Neighbors (KNN): Classifies based on feature similarity.
- Support Vector Classifier (SVC): Effective for high-dimensional data.
- Multinomial Naive Bayes: A probabilistic learning method.

## Results
The models achieve high precision and recall across all classes, with specific performance metrics (Accuracy, F1-score) detailed within the notebook for each algorithm. 
The Decision Tree and Logistic Regression models show particularly strong performance in differentiating these celestial bodies.
