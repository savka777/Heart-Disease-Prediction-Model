# Heart Disease Prediction Model

## Project Overview

This project is a collaborative effort to develop a machine learning model capable of predicting the likelihood of heart disease based on various health indicators. The project was undertaken as part of a year-long university course at the University of Essex and involved multiple stages of data preprocessing, exploratory data analysis, model building, and evaluation.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Preprocessing](#data-preprocessing)
- [Model Development](#model-development)
- [Model Evaluation](#model-evaluation)
- [Feature Selection](#feature-selection)
- [Results](#results)
- [Technologies Used](#technologies-used)

## Dataset

The dataset used in this project is a collection of medical data related to heart disease. It includes the following features:
- **Age:** The age of the patient.
- **Sex:** The gender of the patient (0 = female, 1 = male).
- **Chest Pain Type:** Type of chest pain experienced by the patient.
- **Resting Blood Pressure:** Resting blood pressure (in mm Hg).
- **Cholesterol:** Serum cholesterol in mg/dl.
- **Fasting Blood Sugar:** Fasting blood sugar level (0 = <120 mg/dl, 1 = >120 mg/dl).
- **Resting ECG:** Resting electrocardiographic results.
- **Max Heart Rate:** Maximum heart rate achieved.
- **Exercise Induced Angina:** Exercise-induced angina (1 = yes, 0 = no).
- **ST Depression:** Depression induced by exercise relative to rest.
- **ST Slope:** The slope of the peak exercise ST segment.
- **Number of Major Vessels:** Number of major vessels colored by fluoroscopy.
- **Thallium Stress Test:** Results of a Thallium stress test.
- **Condition:** Diagnosis of heart disease (1 = presence, 0 = absence).

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis was conducted to understand the distribution of data and the relationships between features. Key visualizations include:

- **Condition Ratio:** A pie chart showing the distribution of patients with and without heart disease.
- **Sex Ratio:** A pie chart depicting the gender distribution within the dataset.
- **Risk Factors:** Bar charts and distribution plots for key risk factors such as fasting blood sugar, resting blood pressure, cholesterol levels, and maximum heart rate.

## Data Preprocessing

The data preprocessing steps included:

- **Renaming Columns:** The original column names were renamed for clarity.
- **Missing Values:** The dataset was checked for missing values, and appropriate handling methods were applied.
- **Encoding Categorical Variables:** The target variable (Condition) was label-encoded to facilitate model training.
- **Train-Test Split:** The dataset was split into training (80%) and testing (20%) sets.
- **Normalization:** Features were normalized using `MinMaxScaler` to ensure that all values are within the same range.

## Model Development

Several machine learning models were developed and evaluated:

- **Logistic Regression:** A simple linear model used as a baseline.
- **Random Forest Classifier:** An ensemble method that uses multiple decision trees to improve prediction accuracy.
- **Support Vector Machine (SVM):** A model that finds the optimal hyperplane to separate data into different classes.
- **XGBoost:** A gradient boosting algorithm known for its performance in classification tasks.

## Model Evaluation

Model performance was evaluated using several metrics:

- **Accuracy:** The percentage of correct predictions out of total predictions.
- **Confusion Matrix:** A matrix showing true positives, true negatives, false positives, and false negatives.
- **Classification Report:** A detailed report including precision, recall, F1-score, and support for each class.

## Feature Selection

Feature selection was performed using:

- **RandomForestClassifier:** Used to determine feature importance and select the most relevant features.
- **SelectFromModel:** A method used to reduce the feature set to only the most significant predictors, improving model efficiency and interpretability.

## Results

The following table summarizes the accuracy of different models before and after hyperparameter tuning:

| Model                    | Accuracy Before Tuning (%) | Accuracy After Tuning (%) |
|--------------------------|----------------------------|---------------------------|
| Logistic Regression       | 85.25                      | 86.89                      |
| Random Forest Classifier  | 81.97                      | 86.89                      |
| Support Vector Machine    | 85.25                      | 88.52                      |
| XGBoost Classifier        | 86.89                      | 81.97                      |


## Technologies Used

- **Python:** The programming language used for all aspects of the project.
- **Pandas:** For data manipulation and analysis.
- **Scikit-learn:** For implementing machine learning algorithms and preprocessing.
- **XGBoost:** For advanced model building.
- **Matplotlib & Seaborn:** For data visualization.
- **Google Colab:** For collaboration and cloud-based execution.

