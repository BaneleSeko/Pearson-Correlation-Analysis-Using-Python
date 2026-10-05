# Syntecxhub Project 3 - Correlation Heatmap & Pairwise Relationships

## Project Overview

This project analyzes sales data using Python to investigate relationships between
different sales order features.

The analysis focuses on Pearson correlation, correlation heatmaps, pairwise
relationships, and scatter plots to identify strong positive and negative
relationships within the data.

## Dataset

The project uses a sales dataset containing sales order information such as:

- Sales Order Number
- Sales Order Line Number
- Order Date
- Customer Name
- Item
- Quantity
- Unit Price
- Tax Amount

For the correlation analysis, the original sales data was aggregated at the
order level to create more meaningful features.

## Features Analyzed

The following features were used:

- `OrderLineCount` - Number of sales lines within an order
- `TotalSales` - Total sales value of an order
- `AvgUnitPrice` - Average unit price within an order

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Analysis Performed

### 1. Pearson Correlation

Pearson correlation was calculated to measure the strength and direction of
relationships between the numeric sales features.

### 2. Correlation Heatmap

A correlation heatmap was created to visually represent the relationships
between the features.

The upper triangle of the heatmap was masked and the correlation values were
annotated.

### 3. Pairplot

A pairplot was created to examine pairwise relationships between the selected
sales features.

### 4. Scatter Plot

A focused scatter plot was created to visualize the relationship between
`AvgUnitPrice` and `TotalSales`.

## Key Findings

### Strongest Positive Relationship

`TotalSales` and `AvgUnitPrice` had the strongest positive correlation:

**Pearson correlation: 0.905**

This indicates a strong positive relationship between average unit price and
total sales value at the order level.

### Strongest Negative Relationship

`OrderLineCount` and `AvgUnitPrice` had the strongest negative correlation:

**Pearson correlation: -0.526**

This indicates a moderate negative relationship between the number of order
lines and the average unit price.

### Other Relationship

`OrderLineCount` and `TotalSales` showed a weak negative correlation:

**Pearson correlation: -0.261**

## Project Structure

```text
Syntecxhub_Project_3/
│
├── sales.csv
├── analysis.ipynb
├── analysis.py
├── README.md
│
└── Plots/
    ├── correlation_heatmap.png
    ├── pairplot.png
    └── scatter_plot.png

