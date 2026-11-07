# Task 19: Filter Dataset Records using Pandas

## Overview
This project is part of the Veda Technology AI & ML Internship.

The objective of this task is to filter records from a dataset using one or more conditions with Python and Pandas.

The Iris dataset is used to demonstrate Boolean filtering and multiple conditions.

## Objective
Learn how to retrieve relevant records from a dataset using Pandas filtering techniques.

## Dataset Information
- **Dataset:** Iris Dataset
- **File:** `Iris.csv`
- **Total Records:** 150
- **Total Columns:** 6

### Dataset Columns
- Id
- SepalLengthCm
- SepalWidthCm
- PetalLengthCm
- PetalWidthCm
- Species

## Tools & Technologies
- Python
- Pandas
- NumPy
- Google Colab
- Jupyter Notebook

## Filtering Operations Performed

### 1. Filter by Species
Selected all records where the species is `Iris-setosa`.

```python
setosa = df[df['Species'] == 'Iris-setosa']
```
**Result:** 50 records.

### 2. Filter by Sepal Length
Selected flowers with a sepal length greater than 5 cm.

```python
long_sepal = df[df['SepalLengthCm'] > 5]
```
**Result:** 118 records.

### 3. Filter Using AND Condition
Selected flowers where petal length is greater than 4 cm and petal width is greater than 1 cm.

```python
filtered_and = df[
    (df['PetalLengthCm'] > 4) &
    (df['PetalWidthCm'] > 1)
]
```
**Result:** 83 records.

### 4. Filter Using OR Condition
Selected flowers where sepal length is greater than 6 cm or petal length is greater than 5 cm.

```python
filtered_or = df[
    (df['SepalLengthCm'] > 6) |
    (df['PetalLengthCm'] > 5)
]
```
**Result:** 66 records.

## Key Concepts Learned
- Boolean indexing in Pandas
- Filtering records using comparison operators
- Combining multiple conditions using `&` (AND)
- Combining conditions using `|` (OR)
- Retrieving relevant records from a DataFrame
- Counting filtered records

## Project Structure

```text
Filter-Dataset-Records/
│
├── Filter_Dataset_Records.ipynb
├── Iris.csv
└── README.md
```

## How to Run
1. Clone or download this repository.
2. Open `Filter_Dataset_Records.ipynb` in Google Colab.
3. Upload the `Iris.csv` dataset.
4. Make sure the CSV file path in the notebook points to the uploaded dataset.
5. Run all cells to view the filtering results.

## Learning Outcome
Successfully learned how to filter dataset records using Pandas Boolean conditions and retrieve relevant information using single and multiple filtering criteria.

## Internship Details
- **Organization:** Veda Technology
- **Track:** AI & ML Internship
- **Task:** 19 – Filter Dataset Records

