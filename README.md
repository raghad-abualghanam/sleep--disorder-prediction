# Sleep Health and Sleep Disorder Prediction

## Project Overview

This project explores patterns related to sleep health and sleep disorders using data analysis and machine learning.

The main goal is to investigate whether sleep, lifestyle, and health-related variables can help distinguish between different sleep disorder categories.

## Problem

Sleep disorders can be associated with multiple factors such as sleep duration, sleep quality, stress, physical activity, age, and other health-related variables.

This project investigates the following question:

> Can sleep, lifestyle, and health information be used to predict sleep disorder categories?

## Dataset

The project uses the Sleep Health and Lifestyle Dataset.

The dataset contains 374 records and 13 original columns.

The main variables include:

- Gender
- Age
- Occupation
- Sleep Duration
- Quality of Sleep
- Physical Activity Level
- Stress Level
- BMI Category
- Blood Pressure
- Heart Rate
- Daily Steps
- Sleep Disorder

The dataset is synthetic and was created for illustrative purposes.

## Exploratory Data Analysis

The dataset was explored by examining:

- Dataset size and structure
- Missing values
- Duplicate records
- Descriptive statistics
- Variable distributions
- Relationships between sleep-related variables
- Differences between sleep disorder categories

Statistical analysis was also used to investigate relationships between important variables and Sleep Disorder.

## Key Findings

- Sleep Disorder was associated with differences in age, sleep duration, sleep quality, stress level, and physical activity.
- Sleep Duration and Quality of Sleep showed a strong positive relationship.
- Quality of Sleep and Stress Level showed a strong negative relationship.
- Sleep Duration and Stress Level also showed a strong negative relationship.
- Quality of Sleep was associated with Sleep Disorder but was not sufficient to determine the disorder on its own.

## Data Preparation

Person ID was excluded because it is an identifier and does not provide useful predictive information.

Blood Pressure was transformed into two numerical variables:

- Systolic BP
- Diastolic BP

Categorical variables were encoded using One-Hot Encoding.

Numerical variables were standardized using StandardScaler.

## Machine Learning

A Logistic Regression model was used to classify the three Sleep Disorder categories:

- No Disorder
- Insomnia
- Sleep Apnea

A Dummy Classifier was used as a baseline.

The data was divided into training and testing sets.

## Results

The baseline model achieved an accuracy of:

**57.33%**

The Logistic Regression model achieved:

**90.67% test accuracy**

Five-fold Cross-Validation produced a mean accuracy of:

**90.63%**

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Cross-Validation

## Practical Interpretation

The analysis shows that sleep-related, lifestyle, and health variables contain useful patterns for distinguishing between sleep disorder categories in this dataset.

The model can be viewed as an exploratory Data Science tool for identifying patterns in sleep health data.

It should not be considered a medical diagnostic system.

## Limitations

- The dataset is synthetic and should not be treated as clinical data.
- The dataset is relatively small.
- The observed relationships represent associations and do not establish causation.
- Model performance on this dataset does not guarantee similar performance on real-world populations.

## Project Files

- `sleep-disorder-prediction.ipynb` — Complete data analysis and machine learning workflow.
- `Sleep_health_and_lifestyle_dataset.csv` — Dataset used in the project.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Author

raghad-abualghanam
