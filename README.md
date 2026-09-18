# 🚢 Titanic Survival Prediction

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Logistic%20Regression-orange)
![Kaggle](https://img.shields.io/badge/Kaggle-Titanic-20BEFF)

## 📌 Project Overview

This project is a machine learning solution for the Kaggle competition:

**Titanic - Machine Learning from Disaster**

The goal is to predict whether a passenger survived the Titanic disaster based on passenger information.

This project follows a complete machine learning workflow:

```
Data Exploration
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Model Training
        ↓
Validation
        ↓
Kaggle Submission
```

---

# 📊 Dataset

The dataset contains passenger information including:

| Feature | Description |
|---|---|
| Pclass | Passenger class |
| Sex | Passenger gender |
| Age | Passenger age |
| SibSp | Number of siblings/spouses aboard |
| Parch | Number of parents/children aboard |
| Fare | Ticket fare |
| Embarked | Port of embarkation |

Training data:

```
891 passengers
12 features
```

---

# 🔍 Exploratory Data Analysis

## Survival Distribution

The training dataset contains:

- Survived: 342 passengers
- Not survived: 549 passengers

Overall survival rate:

```
38.38%
```

---

## Key Findings

### 👩 Gender Effect

Female passengers had a significantly higher survival rate compared with male passengers.

### 🎫 Passenger Class

Higher-class passengers generally showed higher survival rates.

### 👨‍👩‍👧 Family Size

A new feature was created:

```
FamilySize = SibSp + Parch + 1
```

The survival pattern showed:

| Family Type | Survival Rate |
|---|---|
| Alone | 30.35% |
| Small Family (2-4 people) | 57.88% |
| Large Family (5+ people) | 16.13% |

Small families showed better survival outcomes compared with alone travelers and large families.

---

# 🛠 Feature Engineering

## 1. Title Extraction

Passenger names were processed to extract titles:

```
Mr
Mrs
Miss
Master
Rare
```

This captured social information contained in names.

---

## 2. Family Type

Family size was transformed into categorical features:

```
Alone
Small Family
Large Family
```

This helped the model capture different survival patterns among passengers.

---

# 🤖 Machine Learning Model

## Logistic Regression

Logistic Regression was selected because:

- It is suitable for binary classification problems.
- It is easy to interpret.
- Model coefficients provide insights into feature importance.

Features used:

```
Pclass
Sex
Age
Fare
Embarked
Title
FamilyType
```

---

# 📈 Results

## Validation Performance

Accuracy:

```
83.80%
```

## Kaggle Submission

Public Score:

```
0.77511
```

---

# 💻 Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Kaggle Notebook
- GitHub

---

# 📂 Project Structure

```
Titanic-Survival-Prediction

│
├── Titanic-Survival-Prediction.ipynb
│
└── README.md
```

---

# 📚 What I Learned

Through this project, I learned:

- How to explore and clean real-world datasets.
- How feature engineering improves machine learning performance.
- How to build an end-to-end machine learning workflow.
- Why validation results may differ from Kaggle leaderboard results.

---

⭐ This is my first Kaggle machine learning project.
