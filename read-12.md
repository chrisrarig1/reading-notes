# Pandas

## Import

- `In [1]: import numpy as np`
- `In [2]: import pandas as pd`

## Object Creation

- **Series**: Pass a list of values
- `In[3]: s = pd.Series([#,#,#, np.nan])`
- **DataFrame**: Pass a NumPy array
- `In [5]: dates = pd.date_range("20130101, periods=6)`
- A Dictionary of objects can be passed through
- `pd.DataFrame({"A":1.0,"B":data})`
- Use `dtypes` to see data types

## Viewing Data

- `.head()`: Allows us to view the top rows
- `.tail(#)`: Allows us to see the bottom rows
- `.index`: Displays the indexes
- `.columns`: Displays columns
- `.to_numpy()`: This forces all data to have one data type
- `describe()`: Shows a quick statistic summary of data
- `.T`: Transposes data
- `.sort_index(axis=1, ascending=False)`: Sort by an axis
- `sort_values(by="B")`: Sort by values

## Getting

- `df["A"]`: Getting columns
- `df[:]`: Splicing for rows

## Selection by Label

- `.loc[row label[0]]`:for getting the cross section using a label.

## Selection by position

- `.iloc[3]`: Select via position of passed integers
- `.iloc[3:5, 0:2]`: Select by slicing

## Boolean Indexing

- `df[df["A"]>0]`: Using a single column's values to select data

# Useful Links

- [Pandas](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)
- [What Is Pandas](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)