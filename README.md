# Titanic Survival Prediction Using Decision Trees

## Overview
This project builds a machine learning model to predict passenger survival on the Titanic using a Decision Tree Classifier. It follows a complete machine learning workflow including data preparation, model training, hyperparameter tuning, and evaluation.  
Although inspired by a Udacity lab, the project has been personalized and extended.

## Problem Statement
The goal is to predict whether a passenger survived the Titanic disaster based on available features.  
This is a binary classification problem where:
- 1 indicates survival
- 0 indicates non survival

## Dataset
The dataset contains demographic and ticket-related information of Titanic passengers.  
Target variable: `Survived`

Dataset path: Data/titanic_data.csv

## Methodology

### Data Preparation
- Selected relevant features
- Separated features X and target y
- Split data into training and test sets using an 80 20 split

### Model Training
A Decision Tree Classifier was trained on the training set.  
Initial training resulted in perfect training accuracy, indicating overfitting.

### Hyperparameter Tuning
To improve generalization, GridSearchCV was used to tune the model.

Best parameters found:
- max_depth: 7  
- min_samples_split: 15  
- min_samples_leaf: 4  

## Model Performance

- Training accuracy: 87.9%
- Test accuracy: 84.9%

The close performance between training and test sets suggests a well-regularised model.

## Feature Importance
Feature importance analysis shows that variables such as passenger sex, ticket class, and age play a significant role in predicting survival, which aligns with historical insights.

## Tools and Libraries
- Python
- pandas
- numpy
- scikit learn
- matplotlib

## Project Structure

```
titanic-survival-decision-tree/
│
├── Data/
│ └── titanic_data.csv
│
├── titanic_survival_decision_tree.ipynb
├── README.md
└── .gitignore/
```

## Key Learnings
- Building and tuning decision tree models
- Using grid search to reduce overfitting
- Evaluating models using training and test accuracy
- Interpreting feature importance

## Future Improvements
- Try ensemble methods like Random Forest or Gradient Boosting
- Evaluate additional metrics such as precision, recall, and F1 score
- Perform more feature engineering

## Author
Musediku Oluwafisayomi  
Aspiring Data Scientist and Machine Learning Practitioner

