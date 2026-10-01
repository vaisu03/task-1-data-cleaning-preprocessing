# Task 1 - Data Cleaning & Preprocessing

## AI & ML Internship

This project demonstrates data cleaning and preprocessing using the Titanic dataset.

## Objective

The objective of this task is to learn how to clean and prepare raw data for machine learning.

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

## Dataset

The Titanic dataset was used for this task.

## Preprocessing Steps

### 1. Dataset Exploration

* Loaded the Titanic dataset using Pandas.
* Examined the dataset shape.
* Checked data types.
* Checked for missing values.
* Generated descriptive statistics.

### 2. Missing Value Handling

* Removed the `Cabin` column because of its large amount of missing information.
* Removed `PassengerId` because it is an identifier.
* Filled missing `Age` values using median imputation.
* Filled missing `Embarked` values using mode imputation.

### 3. Categorical Encoding

Categorical features were converted into numerical features using one-hot encoding.

The `Sex` and `Embarked` columns were encoded using Pandas `get_dummies()`.

### 4. Outlier Detection

Boxplots were used to visualize potential outliers.

The Interquartile Range (IQR) method was used to identify outliers in the `Fare` feature.

### 5. Outlier Removal

Fare values outside the IQR-based lower and upper bounds were removed.

### 6. Feature Scaling

`StandardScaler` from Scikit-learn was used to standardize the `Age` and `Fare` features.

### 7. Processed Dataset

The final cleaned dataset was saved as:

`titanic_cleaned.csv`

## Project Files

* `Task_1_Data_Cleaning_Preprocessing.ipynb` - Google Colab notebook containing the complete implementation.
* `titanic_cleaned.csv` - Processed Titanic dataset.
* `README.md` - Project documentation.

## Key Learning

Data preprocessing is an important step in machine learning because raw datasets may contain missing values, categorical variables, outliers, and features with different scales. Proper preprocessing prepares the data for further machine learning tasks.

## Conclusion

This task provided practical experience with data exploration, missing-value handling, categorical encoding, outlier detection and removal, and feature standardization using Python.
