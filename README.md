# Prediction-of-Solar-System-Coverage

![shutterstock_612543161-1-800x400](https://github.com/sarveshsn/Prediction-of-Solar-System-Coverage/assets/93898181/ea5f1513-5fb5-49a6-9530-c7a1cdfc5595)


## Year: 2023

**Table of Contents**
- [Introduction](#introduction)
- [Data](#data)
- [Models](#models)
  - [Logistic Regression Model](#logistic-regression-model)
  - [Random Forest Model](#random-forest-model)
  - [Support Vector Machine (SVM)](#support-vector-machine-svm)
  - [Classification Trees](#classification-trees)
- [Model Comparison](#model-comparison)
- [Generalized Predictive Performance](#generalized-predictive-performance)

## Introduction
This repository presents the prediction of solar system coverage using supervised learning methods. The goal is to determine if a given tile has high or low solar power system coverage based on input features. Four different supervised learning methods are implemented and evaluated, followed by a model comparison to select the best-performing model. Finally, the generalized predictive performance of the selected model is assessed.

## Data
The dataset used contains 10,926 observations and 15 numeric variables. The target variable is `solar_system_coverage`, and all other variables are considered predictor variables. There are no missing values in the dataset.

### Load Data
```R
load('data_deepsolar.RData')
str(data)
any(is.na(data))
```

## Models

### Logistic Regression Model
A logistic regression model is used to predict solar system coverage. The model's deviance, coefficients, sensitivity-specificity plot, precision-recall curve, and F1 score are analyzed.

### Random Forest Model
A random forest model is implemented and evaluated. The model's confusion matrix, feature importance, accuracy, sensitivity, specificity, and F1 score are examined.

### Support Vector Machine (SVM)
Two SVM models with different kernels (polynomial and sigmoid) are trained and assessed. Performance metrics such as accuracy, sensitivity, specificity, precision, recall, F1 score, and AUC are calculated.

### Classification Trees
A classification tree model is constructed, and its performance is evaluated using metrics like accuracy, sensitivity, specificity, precision, recall, F1 score, and AUC. A pruned tree is also visualized.

## Model Comparison
Performance metrics from different models are compared to select the best-performing model. Random Forest emerges as the top-performing model based on accuracy and AUC.

## Generalized Predictive Performance
The selected Random Forest model is evaluated using a separate test dataset. Performance metrics including accuracy, sensitivity, specificity, and AUC are assessed to gauge the model's predictive power.

For more details, please refer to the individual sections and R code provided in this repository.


## Author 

- **Sarvesh Sairam Naik**
