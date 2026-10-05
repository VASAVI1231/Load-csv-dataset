## Load a CSV Dataset Using Pandas

### Project Overview

This project is part of the VEDA Technology AI & ML Internship.

The objective of this task is to learn how to load a real-world CSV dataset using Python and Pandas.

For this project, the Iris dataset is used. The dataset is loaded directly from a public CSV source and converted into a Pandas DataFrame.

---

## Objective

- Learn how to work with CSV datasets.
- Load a CSV file using Pandas.
- Display the first five records.
- Display the last five records.
- Check the dataset shape.
- Check column names.
- Check for missing values.

---

## Dataset

The Iris dataset contains measurements of iris flowers.

It contains:

- 150 records
- 4 numerical features
- 1 target/species column
- 3 iris species

### Features

1. Sepal Length
2. Sepal Width
3. Petal Length
4. Petal Width

### Species

- Iris-setosa
- Iris-versicolor
- Iris-virginica

---

## Technologies Used

- Python
- Pandas
- Google Colab
- GitHub

---

## Python Code

```python
import pandas as pd

url = "https://raw.githubusercontent.com/jbrownlee/Datasets/master/iris.csv"

columns = [
    "sepal_length",
    "sepal_width",
    "petal_length",
    "petal_width",
    "species"
]

df = pd.read_csv(url, names=columns)

print("Dataset loaded successfully!")

print("\nFirst 5 Records:")
print(df.head())

print("\nLast 5 Records:")
print(df.tail())

print("\nDataset Shape:")
print(df.shape)

print("\nColumn Names:")
print(df.columns.tolist())

print("\nMissing Values:")
print(df.isnull().sum())

print("\nDataset Information:")
print(df.info())

## Expected Result
The dataset should be successfully loaded into a Pandas DataFrame.
The dataset shape is:
(150, 5)
The first five and last five records can be displayed using:
df.head()
df.tail()

## Dataset Source
UCI Machine Learning Repository:
https://archive.ics.uci.edu/dataset/53/iris⁠�
CSV source:
https://github.com/jbrownlee/Datasets/blob/master/iris.csv⁠�

## Conclusion
The Iris dataset was successfully loaded using Pandas.
The first and last records were displayed, the dataset shape was checked, column names were inspected, and missing values were verified.
This project provides a basic understanding of loading and inspecting datasets before performing data preprocessing and machine learning tasks.
