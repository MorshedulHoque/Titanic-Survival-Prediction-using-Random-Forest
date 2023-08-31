# Titanic-Survival-Prediction-using-Random-Forest

# Titanic Survival Prediction

## Introduction

The Titanic Survival Prediction project revolves around exploring the historical Titanic dataset to understand the factors that influenced the passengers' chances of survival. By utilizing machine learning techniques, we aim to build a predictive model that can classify whether a passenger survived the disaster or not.

## Objective

- Analyze the Titanic dataset to identify patterns related to passenger survival.
- Build and fine-tune a classification model to predict passenger survival based on available features.
- Compare the performance of various classification algorithms.

## Project Overview

The sinking of the Titanic on April 15, 1912, was a tragic event that resulted in the loss of many lives. This project uses modern data analysis and machine learning methods to gain insights into the characteristics that contributed to survival during this catastrophe.

### Key Steps

1. **Data Exploration and Cleaning**: We began by understanding the structure of the dataset and addressing any missing or inconsistent data. This ensures the dataset is suitable for training a machine learning model.

2. **Feature Engineering**: We selected relevant features such as age, gender, and socio-economic class that could potentially influence survival outcomes. Categorical variables were one-hot encoded for model compatibility.

3. **Model Selection and Training**: We employed the RandomForestClassifier to predict survival. The initial model was trained using the training dataset.

```python
# Example code for model training
from sklearn.ensemble import RandomForestClassifier

model = RandomForestClassifier(n_estimators=100, max_depth=5, random_state=1)
model.fit(X_train, y_train)
