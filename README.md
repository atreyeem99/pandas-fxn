# pandas-fxn
## Data Structures:
```
    Series: One-dimensional labeled array.
    DataFrame: Two-dimensional labeled data structure with columns of potentially different types.
```
## pd.describe()
```
describe(): Generate descriptive statistics of DataFrame.
```
## head(): 
```
View the first n rows of the DataFrame.
```
## tail():
```
View the last n rows of the DataFrame.
```
## info(): 
```
Get concise summary of DataFrame including data types and missing values.
```
## shape:
```
Return a tuple representing the dimensionality of the DataFrame.
```
## dtypes: 
```
Return the data types of each column.
```
## columns: 
```
Return the column labels of the DataFrame.
```
## index: 
```
Return the index (row labels) of the DataFrame.
```
# I/O Functions:

  ##  read_csv(): Read a CSV file into a DataFrame.
  ## read_excel(): Read an Excel file into a DataFrame.
  ## at[]: Access a single value for a row/column label pair.
  ## iat[]: Access a single value for a row/column pair by integer position.
  ## query(): Filter rows from a DataFrame that meet a specified condition.
  to_excel(): Write a DataFrame to an Excel file.

# Data Manipulation:

    ## merge(): Merge DataFrame objects by performing a database-style join operation.
    ## concat(): Concatenate pandas objects along a particular axis.
    ## drop(): Drop specified labels from rows or columns.
    ## groupby(): Group DataFrame using a mapper or by a Series of columns.
    ## pivot_table(): Create a spreadsheet-style pivot table as a DataFrame 
    ## stack() and unstack(): Reshape a DataFrame by pivoting the index labels
Data Cleaning:

    fillna(): Fill missing values with specified methods.
    dropna(): Remove missing values from DataFrame.
    eplace(): Replace values in DataFrame with other values.
Data Analysis:

    value_counts(): Count distinct values in a Series.
    unique(): Return unique values in a Series.
    nunique(): Return number of unique elements in a Series.
to_csv(): Write a DataFrame to a CSV file.
to_excel(): Write a DataFrame to an Excel file.


```
import pandas as pd

# Read the CSV file into a DataFrame
df = pd.read_csv('your_file.csv')

# Print the second column
print(df.iloc[:, 1])
```
# EXAMPLE 
```
import pandas as pd

# Creating a DataFrame from a dictionary
data = {
    'Name': ['Alice', 'Bob', 'Charlie', 'David'],
    'Age': [25, 30, 35, 40],
    'City': ['New York', 'Los Angeles', 'Chicago', 'Houston']
}

df = pd.DataFrame(data)
print("Original DataFrame:")
print(df)
print()

# Basic DataFrame operations
print("Shape of DataFrame:")
print(df.shape)  # Shape of the DataFrame (rows, columns)
print()

print("Columns of DataFrame:")
print(df.columns)  # Columns of the DataFrame
print()

print("Data types of DataFrame:")
print(df.dtypes)  # Data types of each column
print()

print("Descriptive statistics of numeric columns:")
print(df.describe())  # Summary statistics of numeric columns
print()

# Accessing specific columns
print("Accessing 'Name' column:")
print(df['Name'])
print()

# Adding a new column
df['Gender'] = ['Female', 'Male', 'Male', 'Male']
print("DataFrame after adding 'Gender' column:")
print(df)
print()

# Filtering data based on conditions
print("Filtering data where Age > 30:")
print(df[df['Age'] > 30])
```
