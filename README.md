
#  Decision Trees and Random Forests

This repository contains code and documentation for predicting heart disease using Decision Tree and Random Forest classifiers, as part of a machine learning assignment.

## Overview

We use the UCI Heart Disease dataset (`heart.csv`) to build and evaluate two types of models:
- **Decision Tree Classifier**
- **Random Forest Classifier**

The project includes:
- **Data preprocessing and exploration**
- **Model training and evaluation**
- **Visualization of decision trees**
- **Feature importance analysis**
- **Cross-validation for robust model assessment**


## Methods for solving the task

1. **Data Loading and Cleaning**
   - Load the dataset
   - Check and remove duplicates
   - Split data into features (`X`) and target (`y`)
2. **Train/Test Split**
   - Stratified split (80% train, 20% test) to preserve class balance
3. **Model Training**
   - **Decision Tree:** Trained with varying depths to analyze overfitting
   - **Random Forest:** Trained with default parameters
4. **Model Evaluation**
   - Accuracy on train and test sets
   - Cross-validation for both models
5. **Visualization and Analysis**
   - Visualize the decision tree using Graphviz
   - Plot feature importances from the Random Forest

## Results

| Model/Depth      | Train Accuracy | Test Accuracy | CV Accuracy   |
|------------------|---------------|---------------|--------------|
| Decision Tree 2  | 0.784         | 0.656         | —            |
| Decision Tree 3  | 0.859         | 0.803         | 0.795        |
| Decision Tree 5  | 0.942         | 0.770         | —            |
| Decision Tree 10 | 1.000         | 0.803         | —            |
| Random Forest    | 1.000         | 0.754         | 0.828        |

- **Feature Importance:** Top predictive features are the  `cp`, `thalach`, `ca`, and `thal`.
- **Overfitting:** Observed as tree depth increases, with train accuracy reaching 1.0 but test accuracy stabilizing.






