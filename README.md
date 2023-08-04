# Financial-Dataset-Insights-By-Python.
Explore Financial Insights: Python script analyzes financial data using Pandas, NumPy, Matplotlib, Seaborn.
Detects missing values, duplicates; visualizes via histograms, scatter plots, heatmaps. Investigates mean units sold by country with bar plot.
A concise demo of data analysis, aiding decisions and trend comprehension.

Let's break down the script step by step:

1.Importing Libraries: The script starts by importing the necessary libraries, including Pandas, NumPy, Matplotlib, and Seaborn.

2.Loading Data: The script loads the financial data from the specified CSV file using Pandas' read_csv() function. The dataset seems to have 700 rows and 16 columns.

3.Displaying Data: The script displays the first few rows of the loaded dataset using the head() function to give an overview of the data structure.

4.Data Cleaning and Exploration:
  The script checks the column names using df.columns.
  It checks the data types of columns using df.dtypes.
  It generates summary statistics using df.describe().
  It selects specific columns for further analysis, excluding some columns.

5.Missing Values Check: The script checks for missing values in the dataset using df.isna().sum().

6.Duplicate Rows Check: The script checks for duplicate rows using df.duplicated().

7.Data Visualization:
  The script creates various types of plots using Matplotlib and Seaborn to visualize the data distribution and relationships:
  Histogram ('Units Sold')
  Kernel Density Estimate plot ('Units Sold')
  Scatter plot ('Units Sold' vs 'Country')
  Scatter plot with color encoding by year ('Units Sold' vs 'Country')
  Pair plot ('Units Sold', 'Country', 'Year', and 'Month Number') - though the code snippet for this plot is provided before the variable definition.
  Correlation Heatmap for selected columns ('Units Sold', 'Year', 'Month Number')

8.Visualization: Mean Units Sold by Country: The script calculates the mean units sold for different countries using the groupby() function and then creates a bar plot using Seaborn to visualize the mean units sold for each country.
