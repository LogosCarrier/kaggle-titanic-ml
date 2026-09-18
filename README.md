# Titanic Survival Prediction

## Project Overview

This project is based on the Kaggle Titanic competition.

The goal is to predict whether a passenger survived the Titanic disaster using machine learning models.

## Dataset

Dataset:
Kaggle Titanic - Machine Learning from Disaster

Features include:
- Passenger class
- Sex
- Age
- Fare
- Family information
- Embarked port

## Data Analysis

Explored survival patterns based on:

- Sex
- Passenger class
- Age
- Family size
- Passenger title

Main findings:
- Female passengers had higher survival rates.
- First-class passengers had higher survival rates.
- Small families showed better survival rates than alone travelers or large families.

## Feature Engineering

Created new features:

- Title extracted from passenger names
- FamilySize = SibSp + Parch + 1
- FamilyType:
  - Alone
  - Small
  - Large

## Model

Used:

- Logistic Regression

## Results

Validation Accuracy:
83.80%

Kaggle Public Score:
0.77511

## Tools

- Python
- Pandas
- NumPy
- Scikit-learn
- Kaggle Notebook
