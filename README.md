# health-condition-prediction-using-ml
This repository showcases an end-to-end machine learning project that predicts students' health conditions using  physiological and lifestyle factors. It includes data preprocessing, exploratory data analysis, feature engineering, categorical encoding, and the development and evaluation of classification models.

# Student Health Prediction Using Machine Learning

## Project Overview

This repository presents an end-to-end machine learning project that predicts students' health conditions using physiological, and lifestyle-related factors. The project demonstrates a complete machine learning workflow, including data preprocessing, exploratory data analysis, feature engineering, categorical encoding, model training, evaluation, and prediction on unseen data. 

The objective is to classify students into one of the following health categories:

- Healthy
- At-Risk
- Unhealthy

The models are evaluated using **Balanced Accuracy**, the evaluation metric used in the Kaggle competition.
---

## Dataset

The project uses two datasets provided by the competition:

- **train.csv** – Contains the input features and target variable (`health_condition`).
- **test.csv** – Contains unseen data used to generate final predictions.

### Features

The dataset includes physiological and lifestyle attributes such as:

- Sleep Duration
- Heart Rate
- Body Mass Index (BMI)
- Calorie Expenditure
- Daily Step Count
- Exercise Duration
- Water Intake
- Diet Type
- Stress Level
- Sleep Quality
- Physical Activity Level
- Smoking & Alcohol Consumption
- Gender

---

## Project Workflow

### 1. Data Exploration
- Load and inspect the dataset
- Examine data types
- Detect duplicate records
- Analyze missing values
- Evaluate class distribution

### 2. Data Preprocessing
- Handle missing numerical values
- Impute missing categorical values
- Detect skewness of numerical variables
- Remove duplicate observations

### 3. Feature Engineering

#### Ordinal Encoding
Applied to:

- Stress Level
- Sleep Quality
- Physical Activity Level
- Smoking & Alcohol Consumption

#### One-Hot Encoding
Applied to:

- Gender
- Diet Type

### 4. Exploratory Data Analysis

- Missing value analysis
- Class distribution
- Correlation analysis
- Data quality assessment

### 5. Model Development

The notebook implements:

- Logistic Regression
- Random Forest Classifier

The dataset is divided into training and validation subsets before model training.

### 6. Model Evaluation

Performance is assessed using:

- Balanced Accuracy
- Classification Report
- Confusion Matrix

### 7. Prediction

The trained model is applied to the competition test dataset to generate predictions for submission.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn

---

## Machine Learning Techniques

- Missing Value Imputation
- Ordinal Encoding
- One-Hot Encoding
- Train–Validation Split
- Logistic Regression
- Random Forest Classification
- Balanced Accuracy Evaluation

---

## Repository Structure

```
Student-Health-Prediction-ML/
│
├── student_health_prediction_ML.ipynb
├── submission.csv
├── test.csv
├── README.md

```

---

## Results

The implemented Random Forest classifier achieved a **Balanced Accuracy of approximately 0.85** on the validation dataset, providing a strong baseline for predicting student health conditions.

---

## Future Improvements

Potential enhancements include:

- Hyperparameter optimization using GridSearchCV or RandomizedSearchCV
- Feature selection techniques
- Cross-validation
- Model comparison with XGBoost, LightGBM, and CatBoost
- Automated preprocessing pipelines

---

Master of Science in Data Science  
Hofstra University
