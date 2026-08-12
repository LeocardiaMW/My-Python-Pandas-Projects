# Python Pandas Data Analysis Project

## Overview

This project was completed during a **Data Technician Bootcamp** and focused on using **Python Pandas** to explore, clean, manipulate, analyse, and visualize retail and sales datasets. The project developed practical data analysis skills through working with real-world datasets, applying data cleaning techniques, filtering records, generating insights, and creating visualizations to support decision-making.

## Objectives

- Import and analyse retail and sales datasets using Pandas.
- Clean and prepare data for analysis.
- Filter and select relevant business information.
- Perform data transformations and aggregations.
- Identify trends and patterns within sales data.
- Create visualizations to communicate insights effectively.
- Develop foundational skills used in data analytics workflows.

## Tools and Technologies

- Python
- Pandas
- Matplotlib
- Google Colab
- CSV Datasets
- Jupyter Notebook Environment

## Pandas Skills Demonstrated

### Data Import and Exploration

Loaded datasets into Pandas DataFrames and explored their structure using:

```python
import pandas as pd

df = pd.read_csv("sales_data.csv")

df.head()
df.info()
df.describe()
```

This provided an understanding of dataset contents, column types, and overall data quality.

---

### Filtering Data

Used filtering techniques to analyse specific subsets of data, such as:

- High-value sales
- Products from specific categories
- Regional sales performance
- Customer-specific transactions

```python
high_sales = df[df["Sales"] > 1000]
```

Filtering allowed focused analysis and targeted business insights.

---

### Data Selection with `.loc[]`

Used `.loc[]` to select data by labels and apply conditional filtering.

```python
df.loc[df["Region"] == "North", ["Product", "Sales"]]
```

This enabled efficient retrieval of relevant records and columns for reporting and investigation.

### ✨📸 example:

<img width="857" height="122" alt="image" src="https://github.com/user-attachments/assets/bf8dd9cd-5926-4843-99e8-4940f5f06d3d" />



---

### Data Selection with `.iloc[]`

Used `.iloc[]` to access data by row and column positions.

```python
df.iloc[0:10, 0:3]
```

This provided precise control when inspecting specific sections of large datasets.

---

### Grouping and Aggregation with `groupby()`

Grouped business data to generate meaningful summaries.

```python
df.groupby("Category")["Sales"].sum()
```

Applications included:

- Total sales by category
- Revenue by region
- Customer purchase summaries
- Product performance comparisons

---

### Sorting Data with `sort_values()`

Organised data to identify top and bottom performers.

```python
df.sort_values("Sales", ascending=False)
```

This was useful for:

- Finding best-selling products
- Ranking regions by revenue
- Identifying high-value customers

---

### Handling Missing Data with `dropna()`

Removed incomplete records when necessary.

```python
df.dropna()
```

This improved data quality and ensured more reliable analysis results.

---

### Handling Missing Data with `fillna()`

Replaced missing values with appropriate defaults.

```python
df.fillna(0)
```

This helped preserve datasets while maintaining consistency for calculations and reporting.

---

### Additional Data Manipulation Techniques

Applied various Pandas methods to transform and prepare data, including:

- Column creation
- Renaming fields
- Changing data types
- Removing duplicates
- Calculating derived metrics
- Aggregating results

```python
df["Profit"] = df["Revenue"] - df["Cost"]
```

These techniques supported deeper analysis and improved dataset usability.

## Data Cleaning Process

A structured cleaning workflow was used to prepare retail and sales data:

1. Load and inspect datasets
2. Identify missing values
3. Remove duplicates
4. Correct data types
5. Handle null values
6. Validate records
7. Prepare data for analysis

This process ensured data accuracy and improved the reliability of analytical results.

## Data Analysis Performed

Using retail and sales datasets, analysis included:

- Product sales performance
- Revenue trends
- Regional sales comparisons
- Customer purchasing behaviour
- Category performance analysis
- Profit calculations
- Sales ranking and segmentation

These analyses helped demonstrate how data can be transformed into actionable business insights.

## Data Visualization

Visualizations were created using Pandas plotting functionality and Matplotlib.

### Sales Trends

```python
df.groupby("Month")["Sales"].sum().plot()
```

### Category Comparison

```python
df.groupby("Category")["Sales"].sum().plot(kind="bar")
```

### Revenue Distribution

```python
df["Revenue"].hist()
```

Visualizations enabled:

- Trend identification
- Performance monitoring
- Comparative analysis
- Clear communication of findings to stakeholders

## Key Learning Outcomes

Through this project, I developed experience in:

- Data exploration and profiling
- Data cleaning and preparation
- Filtering and selecting records
- Using `.loc[]` and `.iloc[]`
- Aggregating data with `groupby()`
- Sorting datasets with `sort_values()`
- Managing missing values using `dropna()` and `fillna()`
- Creating business-focused visualizations
- Performing analytical investigations using Pandas
- Interpreting and presenting data-driven insights

## Example Business Insights

Analysis revealed valuable information such as:

- Top-performing products and categories
- Regions generating the highest sales revenue
- Seasonal sales patterns and trends
- Customer groups contributing most to revenue

These findings demonstrated how Pandas can be used to support operational and strategic business decisions.

## Conclusion

This Python Pandas project strengthened my ability to work with real-world retail and sales data throughout the complete analytics lifecycle. By using filtering techniques, `.loc[]` and `.iloc[]` indexing, aggregation methods such as `groupby()`, data cleaning functions including `dropna()` and `fillna()`, and data visualizations with Pandas and Matplotlib, I gained practical experience in transforming raw data into meaningful insights and reports. The project provided a solid foundation in data analysis, data preparation, and business intelligence using Python.

## ✨📸 Examples of codes and outputs

<img width="874" height="240" alt="image" src="https://github.com/user-attachments/assets/d96d2783-cb0a-4d93-bb22-d15660356d67" />

<img width="868" height="241" alt="image" src="https://github.com/user-attachments/assets/514a9bfe-cd1f-4d8a-a36e-1bc0010f9c51" />

<img width="869" height="251" alt="image" src="https://github.com/user-attachments/assets/91c13e2d-b6af-4713-bc24-a89ea6721931" />

