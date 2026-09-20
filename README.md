# Heart Disease Prediction

## Overview
This project focuses on predicting the presence of heart disease based on various clinical and demographic features. The analysis involves exploring the dataset, understanding feature relationships, and identifying the most significant predictors for heart disease using statistical methods like Pearson Correlation.

## Dataset
The dataset contains 918 records and 12 columns, including various health metrics. The primary target variable for prediction is `HeartDisease`.

## Key Features
Based on the exploratory data analysis and correlation matrix, the dataset incorporates the following metrics (including one-hot encoded variables):

* **Age**
* **Sex** (`Sex_M`)
* **Chest Pain Type** (`ChestPainType_TA`, `ChestPainType_NAP`, `ChestPainType_ATA`)
* **Resting Blood Pressure** (`RestingBP`)
* **Cholesterol**
* **Fasting Blood Sugar** (`FastingBS`)
* **Resting ECG Results** (`RestingECG_ST`, `RestingECG_Normal`)
* **Maximum Heart Rate Achieved** (`MaxHR`)
* **Exercise-Induced Angina** (`ExerciseAngina_Y`)
* **Oldpeak** (ST depression induced by exercise relative to rest)
* **ST Slope** (`ST_Slope_Flat`)

## Technologies Used
* **Python**
* **Pandas:** Data manipulation and DataFrame structuring.
* **SciPy / Stats Libraries:** Pearson correlation calculations (`pearsonr`).
* **Jupyter Notebook:** Interactive data exploration and modeling.

## Key Findings: Feature Correlation
A Pearson Correlation analysis was conducted to understand which features have the strongest linear relationship with the target variable (`HeartDisease`).

**Strongest Positive Correlations:**
* `ST_Slope_Flat`: 0.554
* `ExerciseAngina_Y`: 0.494
* `Oldpeak`: 0.404
* `Sex_M`: 0.305

**Strongest Negative Correlations:**
* `ChestPainType_ATA`: -0.402
* `MaxHR`: -0.400
* `ChestPainType_NAP`: -0.213

## How to Run
1. Ensure you have a Python environment set up (e.g., `conda env:base`) with the required libraries installed (`pandas`, `scipy`, `jupyter`).
2. Open `heart_disease_prediction.ipynb` in Jupyter Notebook or JupyterLab.
3. Run the cells sequentially to reproduce the correlation analysis, view the DataFrames, and execute further predictive modeling steps.
