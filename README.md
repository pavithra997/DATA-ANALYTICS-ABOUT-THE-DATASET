# DATA-ANALYTICS-ABOUT-THE-DATASET
# AIM
To perform data analytics on a given dataset using Python and Pandas, understand the characteristics of the dataset, identify different types of data, examine missing values, and prepare the dataset for further analysis and machine learning.
# THEORY
Data Analytics is the process of examining, cleaning, transforming, and interpreting data to obtain useful information and identify meaningful patterns. It is an important step before applying statistical methods or Machine Learning algorithms.

Python provides several libraries for data analysis, among which Pandas is widely used for handling structured datasets. Pandas provides a DataFrame structure that allows users to easily load, inspect, clean, and analyze data.

The main steps involved in dataset analysis are:

Loading the Dataset – The dataset can be imported using Pandas functions such as read_csv().
Understanding the Dataset – The number of rows, columns, column names, and data types can be identified.
Checking Missing Values – Missing or null values are detected using functions such as isnull().
Statistical Analysis – Functions such as describe() provide statistical information about numerical data.
Data Cleaning – Duplicate records and missing values can be removed or replaced.
Data Visualization – Graphs and charts can be used to understand patterns and relationships in the data.
import pandas as pd

# PYTHON CODE
# Step 1: Load dataset
data = pd.read_csv("dataset.csv")

# Step 2: Display first five records
print("First Five Records:") print(data.head())

# Step 3: Display dataset shape
print("\nDataset Shape:") print(data.shape)

# Step 4: Display column names
print("\nColumn Names:") print(data.columns)

# Step 5: Display data types
print("\nData Types:") print(data.dtypes)

# Step 6: Display information
print("\nDataset Information:") data.info()

# Step 7: Display statistical summary
print("\nStatistical Summary:") print(data.describe())

# Step 8: Check missing values
print("\nMissing Values:") print(data.isnull().sum())

# Step 9: Check duplicate rows
print("\nDuplicate Rows:") print(data.duplicated().sum())

# Step 10: Remove duplicate rows
data = data.drop_duplicates()

print("\nDataset after removing duplicates:") print(data.head())

# RESULT
Thus, data analytics was successfully performed on the given dataset using Python and Pandas. The characteristics, structure, dimensions, data types, missing values, and duplicate records of the dataset were identified.

The dataset was successfully examined and cleaned, making it suitable for further data analysis, visualization, and Machine Learning applications.

# RESULT
