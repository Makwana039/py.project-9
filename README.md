# Sales Data Analyzer

A beginner-friendly Python project for analyzing CSV datasets using
Pandas and NumPy, and creating data visualizations with Matplotlib and
Seaborn. The program uses a menu-driven interface to explore, clean,
analyze, combine, filter, and visualize data.

## Features

-   Load a dataset from a CSV file.
-   Explore the first and last five rows, column names, data types,
    dataset information, missing values, and descriptive summaries.
-   Handle missing values:
    -   Fill missing numeric values with the column mean.
    -   Fill missing text values with the column mode, or `Unknown` when
        no mode is available.
    -   Remove duplicate rows.
-   Perform mathematical operations on numeric columns, including
    addition, multiplication, squaring, and dot products.
-   Split a dataset into two CSV files or combine datasets by rows or
    columns.
-   Search, sort, and filter dataset values.
-   Calculate aggregates such as sum, mean, minimum, maximum, and count.
-   Group numeric values by a category.
-   Generate descriptive statistics, standard deviation, variance,
    percentiles, and correlation matrices.
-   Create pivot tables.
-   Generate bar charts, line charts, scatter plots, pie charts,
    histograms, box plots, correlation heatmaps, and pair plots.
-   Save a line visualization as a PNG, JPG, or JPEG image.

## Requirements

-   Python 3.9 or later recommended
-   pandas
-   NumPy
-   Matplotlib
-   Seaborn

## Installation

1.  Install Python if it is not already installed.

2.  Open a terminal or command prompt in your project folder.

3.  Install the required libraries:

    ``` bash
    pip install pandas numpy matplotlib seaborn
    ```

4.  Save the project code in a Python file, for example
    `sales_data_analyzer.py`.

## How to Run

Run the Python file from your terminal:

``` bash
python sales_data_analyzer.py
```

When prompted, enter the path to your CSV dataset. For example:

``` text
Enter CSV file path: sales_data.csv
```

Use the actual path and filename of your CSV file.

## Main Menu

The program provides these main options:

  Option   Function
  -------- ---------------------------------
  1        Load Dataset
  2        Explore Data
  3        Perform DataFrame Operations
  4        Handle Missing Data
  5        Generate Descriptive Statistics
  6        Data Visualization
  7        Save Visualization
  8        Exit

### DataFrame Operations

The DataFrame Operations submenu includes:

1.  Mathematical Operations
2.  Combine or Split Data
3.  Search, Sort or Filter
4.  Aggregation Functions
5.  Create Pivot Table
6.  Return to Main Menu

### Explore Data

The Explore Data submenu allows you to display:

-   The first five rows
-   The last five rows
-   Column names
-   Data types
-   Basic information, missing-value counts, and descriptive statistics

## Visualization Options

  Chart          Purpose
  -------------- ------------------------------------------------------
  Bar chart      Compare values across rows
  Line chart     Display values as a sequence
  Scatter plot   Explore the relationship between two numeric columns
  Pie chart      Show the distribution of categories
  Histogram      View the distribution of numeric values
  Box plot       Inspect the spread of numeric values
  Heatmap        Visualize correlations between numeric columns
  Pair plot      Compare relationships among multiple numeric columns

## Saving a Visualization

Choose **Save Visualization** from the main menu, enter a numeric
column, and provide an image filename such as `sales_chart.png`. The
filename must end in `.png`, `.jpg`, or `.jpeg`. If no filename is
entered, the program uses `visualization.png`.

The image is saved in the current working directory unless a different
path is provided.

## Project Structure

``` text
Sales-Data-Analyzer/
├── sales_data_analyzer.py
├── sales_data.csv
└── README.md
```

-   `sales_data_analyzer.py` --- Python source code.
-   `sales_data.csv` --- Your input dataset (provide your own file).
-   `README.md` --- Project documentation.

## Libraries Used

-   **Pandas** --- Loads and manipulates tabular data using DataFrames.
-   **NumPy** --- Performs numeric calculations and dot products.
-   **Matplotlib** --- Creates and saves charts.
-   **Seaborn** --- Creates statistical visualizations such as box
    plots, heatmaps, and pair plots.
-   **os** --- Provides file-path information when saving
    visualizations.

## Notes

-   The program expects a CSV dataset that can be read by
    `pandas.read_csv()`.
-   Mathematical operations and statistical calculations use numeric
    columns.
-   Some charts require one or more numeric columns; scatter plots and
    pair plots require at least two.
-   Cleaning changes the dataset currently held in memory. Save a
    separate copy of the original CSV if you need to preserve it.
-   The split operation writes `data_part1.csv` and `data_part2.csv` to
    the current working directory.
-   This project does not automatically save all cleaning or analysis
    changes back to the original CSV file.

## Learning Outcomes

By working on this project, you can practice:

-   Python classes and methods
-   Menu-driven program design
-   Reading CSV files with Pandas
-   Data cleaning and handling missing values
-   NumPy mathematical operations
-   Filtering, sorting, grouping, and aggregation
-   Descriptive statistics and correlation
-   Data visualization and saving charts
-   Basic exception handling

## Author

Add your name here.
