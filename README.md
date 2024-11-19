# Titanic-Prediction
# Titanic Survival Prediction: Kaggle Competition  

This repository contains the implementation of the **Titanic Survival Prediction** project, developed for the Kaggle competition **"Titanic: Machine Learning from Disaster."** The primary objective of the project is to predict whether a passenger survived the Titanic disaster based on features such as age, gender, class, and more. A **Random Forest Classifier** was used to generate the predictions submitted to Kaggle.  

---

## Table of Contents  

1. [Overview](#overview)  
2. [Features](#features)  
3. [Dataset](#dataset)  
4. [Model Used](#model-used)  
5. [Submission File](#submission-file)    
6. [Results](#results)  


---

## Overview  

The Titanic dataset is a well-known dataset in machine learning and is often used to introduce predictive modeling. This project leverages a **Random Forest Classifier** to predict the survival status of passengers based on key features.  

The repository includes:
- Comprehensive data preprocessing and feature engineering.
- Training and evaluation of the Random Forest Classifier.
- Submission generation for Kaggle.  

---

## Features  

- **Data Preprocessing:**  
  - Handling missing values for `Age`, `Cabin`, and `Embarked`.
  - Encoding categorical variables (`Sex`, `Embarked`).
  - Creation of new features (`FamilySize`, `Title`).
  
- **Model Training and Evaluation:**  
  - Implementation of the **Random Forest Classifier.**  
  - Feature importance analysis to identify key predictors.  

- **Submission File Generation:**  
  - Predictions saved in `submissiion.csv` for Kaggle submission.  

---

## Dataset  

The dataset provided by Kaggle includes two main files:  
- **train.csv:** Training data containing features and survival outcomes.  
- **test.csv:** Test data with features for prediction.  

### Key Features  
- **Pclass**: Passenger class (1st, 2nd, 3rd).  
- **Sex**: Gender of the passenger.  
- **Age**: Age of the passenger.  
- **SibSp**: Number of siblings/spouses aboard.  
- **Parch**: Number of parents/children aboard.  
- **Fare**: Ticket fare.  
- **Embarked**: Port of embarkation (C, Q, S).  

### Target Variable  
- **Survived**: Binary (0 = Did not survive, 1 = Survived).  

---

## Model Used  

### Random Forest Classifier  
The Random Forest Classifier was chosen due to its robust performance on classification tasks and ability to handle missing data and categorical variables effectively. Key hyperparameters tuned include:  
- Number of estimators (`n_estimators`).  
- Maximum depth (`max_depth`).  
- Minimum samples per split (`min_samples_split`).  

---

## Submission File  

The submission file, `submissiion.csv`, contains predictions generated by the Random Forest model. It has the following structure:  

| PassengerId | Survived |  
|-------------|----------|  
| 892         | 0        |  
| 893         | 1        |  
| 894         | 0        |  

This format aligns with Kaggle's requirements.  

---


   ```  

---

## Results  

- The Random Forest Classifier achieved strong predictive performance with balanced handling of categorical and numerical features.  
- Feature importance analysis revealed that `Pclass`, `Sex`, and `Fare` were the most influential predictors of survival.  

---
