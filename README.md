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

# Data Manipulation:

    ## merge(): Merge DataFrame objects by performing a database-style join operation.
    ## concat(): Concatenate pandas objects along a particular axis.
    ## drop(): Drop specified labels from rows or columns.
    ## groupby(): Group DataFrame using a mapper or by a Series of columns.
    ## pivot_table(): Create a spreadsheet-style pivot table as a DataFrame 
    ## stack() and unstack(): Reshape a DataFrame by pivoting the index labels
