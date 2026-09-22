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

# PROCEDURE
```
1.Import the Pandas library to work with the dataset.
2.Load the dataset using pd.read_csv() and store it in a DataFrame.
3.Display the first five records using head().
4.Display the shape of the dataset using shape.
5.Display the column names using columns.
6.Display the data types of each column using dtypes.
7.Display complete dataset information using info().
8.Display the statistical summary using describe().
9.Check for missing values using isnull().sum().
10.Check for duplicate rows using duplicated().sum().
11.Remove duplicate rows using drop_duplicates().
12.Display the dataset after removing duplicates.
```

# CODE
```
from google.colab import drive
drive.mount('/content/drive')
import pandas as pd
df = pd.read_csv('/content/drive/My Drive/Data.csv')
df.head()
print("\nDataset Shape:")
print(df.shape)


print("\nColumn Names:")
print(df.columns)


print("\nData Types:")
print(df.dtypes)


print("\nDataset Information:")
df.info()

print("\nStatistical Summary:")
print(df.describe())


print("\nMissing Values:")
print(df.isnull().sum())


print("\nDuplicate Rows:")
print(df.duplicated().sum())


df = df.drop_duplicates()


print("\nDataset after removing duplicates:")
print(df.head())
```

# OUTPUT
<img width="660" height="681" alt="image" src="https://github.com/user-attachments/assets/3880f632-c64a-4f27-a198-9520b657773b" />
<img width="411" height="522" alt="image" src="https://github.com/user-attachments/assets/7aa998f4-5855-4b53-9515-b6bbf8666c27" />

# RESULT
Thus, data analytics was successfully performed on the given dataset using Python and Pandas. The characteristics, structure, dimensions, data types, missing values, and duplicate records of the dataset were identified.

The dataset was successfully examined and cleaned, making it suitable for further data analysis, visualization, and Machine Learning applications.


