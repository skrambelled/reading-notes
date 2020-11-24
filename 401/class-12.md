# Pandas

Pandas is a library for python used for data analysis.

```python
import pandas as pd
```

Pandas uses dataframes as a structure to hold data for analysis.

You can do data visualization, or groupings, change over time, and lots more.

YOu can used numpy with pandas for data collections, or panda can read in data from csv or excel, etc.

## Creating a dataframe

Useing `pd.DataFrame()` you can create dataframes from NumPy arrays, or dictionarys, or other datasets

The coloumns in a dataframe can hold data of different types than other columns.

## Some useful viewing methods

* `df.head()` - shows the first few rows
* `df.tail(n)` - shows the last n rows
* `df.columns` - shows the column headers
* `df.index` - shows the data of index column
* `df.to_numpy()` - convert a dataframe to a numpy data set, which means all the df data *must* be converted the same data type, which may be an object (expensive!).
* `df.T` - transpose data (swap axis)
* `df.sort_index` - sort by axis
* `df.sort_value` - sort by data values

There's too many to list... see [this reference](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

And these [tutorials](https://realpython.com/learning-paths/pandas-data-science/)

[<-- Back](../README.md)
