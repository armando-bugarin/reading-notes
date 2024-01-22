# Read: Class 12

1. **Explain the purpose and basic functionality of the Pandas library. What are some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation?**

Purpose: Pandas is a powerful open-source data manipulation and analysis library for Python. It provides data structures for efficient manipulation and analysis of structured data.

Basic Functionality:

DataFrame: The core data structure, resembling a table or spreadsheet, with rows and columns.

Series: A one-dimensional labeled array, similar to a column in a DataFrame.

Indexing and Selection: Allows for easy indexing and selection of data.

Data Cleaning: Provides functions for handling missing data and cleaning datasets.

Merging and Joining: Enables combining datasets based on common columns.

Grouping and Aggregation: Supports grouping data based on certain criteria and applying aggregate functions.

Time Series Analysis: Contains tools for working with time-series data.

2. **What are the primary data structures in Pandas, and how do they differ in terms of use cases?**

DataFrame: 2-dimensional labeled data structure with columns that can be of different types. It is widely used for data manipulation and analysis.

Series: 1-dimensional labeled array capable of holding any data type. It is often used for representing a single column or row of data.

Panel (Less Common): A 3D data structure that can be used for handling 3D data, but it's less commonly used compared to DataFrames.

Differences:

DataFrames are suitable for handling tabular data with rows and columns.

Series are used for handling one-dimensional data, such as a single column or row.

3. **Describe the process of loading a dataset into a Pandas DataFrame. What are some common file formats that can be used, and which Pandas functions are utilized to read these formats?**

Process:

Use the pd.read_* functions to read data from various file formats.

Common functions include pd.read_csv(), pd.read_excel(), pd.read_json(), etc.

These functions return a DataFrame containing the data from the specified file.

Common File Formats:

CSV (Comma-Separated Values): pd.read_csv('filename.csv')

Excel: pd.read_excel('filename.xlsx')

JSON: pd.read_json('filename.json')

SQL Database: pd.read_sql('SELECT * FROM table', connection)

## `Things I want to know more about`
