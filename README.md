# Diabetes Data Preprocessing

## Overview

This project focuses on preprocessing a diabetes dataset using Python. The dataset is inspected, cleaned, processed for missing values and duplicates, outliers are handled, and the data is transformed for machine learning.

## Dataset

The dataset contains patient information and medical measurements including:

* Gender
* Age
* Urea
* Creatinine
* HbA1c
* Cholesterol
* Triglycerides
* HDL
* LDL
* VLDL
* BMI
* Diabetes Class

## Tasks Performed

### 1. Data Loading and Inspection

* Loaded the dataset using Pandas
* Displayed the first and last rows
* Checked dataset shape and column names
* Checked data types and dataset information
* Identified numerical and categorical columns

### 2. Data Cleaning

* Renamed `ID` to `Visit_ID`
* Renamed `No_Pation` to `Patient_ID`
* Checked unique values in `Gender` and `CLASS`
* Generated statistical summaries
* Identified and handled missing values
* Identified and removed duplicate rows
* Created box plots for numerical variables

### 3. Outlier Handling

* Retained outliers in `AGE`, `HbA1c`, and `BMI`
* Removed `Cr` values above the 99.5th percentile
* Removed `Urea` values above the 99.9th percentile
* Removed extreme outliers from `LDL`, `VLDL`, `HDL`, `TG`, and `Chol` using the IQR method
* Visualized numerical variables after outlier handling

### 4. Data Transformation

* Encoded `Gender` using Label Encoding
* Encoded `CLASS` as the target variable
* Standardized medical features using `StandardScaler`
* Kept `Visit_ID` and `Patient_ID` as identifiers
* Prepared the data for machine learning

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
diabetes-data-preprocessing/
│
├── README.md
├── diabetes_preprocessing.ipynb
└── diabetes.csv
```

## Conclusion

The diabetes dataset was successfully inspected, cleaned, processed for missing values and duplicates, filtered for specified outliers, and standardized for further machine learning applications.

