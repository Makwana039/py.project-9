# Sales Data Analyzer

A beginner-friendly Python project for analyzing, cleaning, processing, and visualizing CSV datasets using Pandas, NumPy, Matplotlib, and Seaborn.

The program provides a menu-driven interface that allows users to explore datasets, handle missing values, perform calculations, combine or split data, generate statistics, create pivot tables, and produce charts.

## Features

- **Load CSV datasets** from a file path.
- **Explore data** by viewing the first and last five rows, column names, data types, and dataset information.
- **Clean data** by filling missing numeric values with the mean, filling missing text values with the mode (or `Unknown` when no mode exists), and removing duplicate rows.
- **Perform mathematical operations**, including addition, multiplication, squaring, and dot products.
- **Combine or split datasets** by rows or columns, or save a dataset as two CSV files.
- **Search, sort, and filter** records using text or numeric conditions.
- **Calculate aggregates**, including sum, mean, minimum, maximum, and count.
- **Group data by category** and summarize numeric values.
- **Generate statistical analysis**, including descriptive statistics, standard deviation, variance, percentiles, and correlations.
- **Create pivot tables** to summarize numeric data by category.
- **Visualize data** with bar charts, line charts, scatter plots, pie charts, histograms, box plots, correlation heatmaps, and pair plots.
- **Save visualizations** as PNG, JPG, or JPEG image files.

## Technologies Used

| Library | Purpose |
| --- | --- |
| Python | Main programming language |
| Pandas | Loading, cleaning, exploring, and manipulating tabular data |
| NumPy | Numeric calculations and array operations |
| Matplotlib | Creating and saving charts |
| Seaborn | Statistical visualizations, including box plots, heatmaps, and pair plots |

## Requirements

- Python 3.9 or a compatible version
- A CSV dataset to analyze
- The Python libraries listed above

## Installation

### 1. Check Python

Open a terminal or command prompt and run:

```bash
python --version
```

### 2. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn
```

### 3. Save the project

Save the Python program in a file such as:

```text
sales_data_analyzer.py
```

## How to Run

Open a terminal in the folder containing the Python file and run:

```bash
python sales_data_analyzer.py
```

When the program starts, choose an option from the main menu.

## Main Menu

```text
========== Data Analysis & Visualization Program ==========
1. Load Dataset
2. Explore Data
3. Perform DataFrame Operations
4. Handle Missing Data
5. Generate Descriptive Statistics
6. Data Visualization
7. Save Visualization
8. Exit
```

### Menu Guide

| Option | Description |
| --- | --- |
| 1. Load Dataset | Load a CSV file by entering its path |
| 2. Explore Data | View rows, column names, data types, information, missing values, and descriptive summaries |
| 3. Perform DataFrame Operations | Open the submenu for calculations, combining or splitting data, searching, sorting, filtering, aggregation, and pivot tables |
| 4. Handle Missing Data | Fill missing values and remove duplicate rows |
| 5. Generate Descriptive Statistics | View statistics and correlations for numeric columns |
| 6. Data Visualization | Generate a selected chart |
| 7. Save Visualization | Save a line chart for a selected numeric column |
| 8. Exit | Close the program |

## DataFrame Operations

The DataFrame Operations submenu contains:

1. **Mathematical Operations** — add a value, multiply by a value, square values, or calculate the dot product of two numeric columns.
2. **Combine or Split Data** — split the current dataset into `data_part1.csv` and `data_part2.csv`, combine another CSV by rows or columns, or display the dataset shape.
3. **Search, Sort or Filter** — search for text, sort a column, or display rows where a numeric value is greater than a specified number.
4. **Aggregation Functions** — calculate sum, mean, minimum, maximum, and count, or group data by category.
5. **Create Pivot Table** — summarize a numeric column by a selected index/category column.
6. **Return to Main Menu** — return to the main menu.

## Supported Visualizations

| Chart | Use |
| --- | --- |
| Bar chart | Compare values across records |
| Line chart | View values across the row index |
| Scatter plot | Examine the relationship between two numeric columns |
| Pie chart | Show the distribution of values in a category column |
| Histogram | Understand the distribution of numeric values |
| Box plot | Inspect spread and potential outliers |
| Correlation heatmap | View correlations between numeric columns |
| Pair plot | Compare pairwise relationships among numeric columns |

## Example Dataset

You can practice with a CSV file such as `sales_data.csv` containing columns like:

```csv
Date,Product,Region,Quantity,Sales,Revenue
2026-01-05,Laptop,West,2,110000,110000
2026-01-08,Mouse,North,5,2500,2500
2026-02-12,Keyboard,South,3,3600,3600
2026-02-18,Monitor,East,1,12000,12000
```

This is only sample data. Your actual CSV file can have different column names and values. Choose column names that exist in your loaded dataset when prompted by the program.

## Data Cleaning Notes

- Missing numeric values are filled with the column mean.
- Missing non-numeric values are filled with the most frequent value (mode). If no mode is available, the program uses `Unknown`.
- Duplicate rows are removed.
- Cleaning changes the dataset currently held in memory. Save a separate CSV copy first if you need to preserve the original data.

## Saving Charts

Choose **Save Visualization** from the main menu, enter a numeric column name, and provide an image filename such as:

```text
sales_chart.png
```

The program supports `.png`, `.jpg`, and `.jpeg`. If you provide only a filename, the image is saved in the current working directory. The program prints the full output path after a successful save.

## Project Structure

```text
Sales-Data-Analyzer/
├── sales_data_analyzer.py
├── sales_data.csv
├── README.md
├── data_part1.csv          # Created when the dataset is split
├── data_part2.csv          # Created when the dataset is split
└── sales_chart.png         # Example saved visualization
```

The CSV files and chart shown above are examples; generated files appear only when you create them.

## Concepts Practiced

- Python classes and objects
- Methods and instance attributes
- Conditional statements and loops
- Exception handling with `try` and `except`
- Pandas DataFrames and Series
- NumPy numeric operations
- Missing-value handling and duplicate removal
- Filtering, sorting, grouping, and aggregation
- Descriptive statistics and correlation
- Pivot tables
- Data visualization with Matplotlib and Seaborn
- Reading and writing CSV files

## Limitations

- The program reads CSV files; it does not directly load Excel workbooks.
- Column names entered at prompts must match the loaded dataset.
- Mathematical operations print results but do not overwrite the selected source column.
- The **Save Visualization** feature saves a line chart for one numeric column, while other chart types are available in the **Data Visualization** menu.
- The dot product requires the two selected numeric columns to have compatible lengths, which they normally do when selected from the same DataFrame.

## Future Improvements

- Add an option to export the cleaned dataset to a new CSV file.
- Add a graphical user interface.
- Allow users to choose more aggregation methods and chart settings.
- Add automated tests and more detailed input validation.
- Add an option to save summary statistics to a report.

## Learning Purpose

This project is designed for Python learners who want hands-on practice with Pandas, NumPy, data analysis, and visualization through a simple command-line application.

## Author

Created as a Python data analysis and visualization learning project.
