# Pandas Trials

An introductory exploratory data analysis (EDA) notebook that demonstrates core Pandas operations for loading, inspecting and summarizing a tabular dataset, using the Big Mart Sales retail data.

## Contents

- [Overview](#overview)
- [Repository Structure](#repository-structure)
- [Dataset](#dataset)
- [Notebook Walkthrough](#notebook-walkthrough)
- [Getting Started](#getting-started)
- [References](#references)

## Overview

Pandas is an open-source Python library for data manipulation and analysis. This project covers the initial inspection steps that come before any cleaning, feature engineering or modelling:

- Reading a CSV file into a DataFrame
- Inspecting dimensions, column names and data types
- Identifying missing values
- Generating descriptive statistics

## Repository Structure

```
Pandas_Trials/
├── 4. Pandas.ipynb            # Introductory Pandas notebook
└── Dataset/
    └── big_mart_sales.csv     # Big Mart Sales dataset
```

## Dataset

**File:** `Dataset/big_mart_sales.csv`

| Property | Value |
|---|---|
| Records | 8,523 |
| Columns | 12 |
| Unique items | 1,559 |
| Outlets | 10 |
| Item categories | 16 |

### Schema

| Column | Type | Description |
|---|---|---|
| `Item_Identifier` | Categorical | Unique product identifier |
| `Item_Weight` | Numeric | Product weight |
| `Item_Fat_Content` | Categorical | Fat content of the product (e.g. Low Fat, Regular) |
| `Item_Visibility` | Numeric | Proportion of total display area allocated to the product |
| `Item_Type` | Categorical | Product category |
| `Item_MRP` | Numeric | Maximum retail price |
| `Outlet_Identifier` | Categorical | Unique outlet identifier |
| `Outlet_Establishment_Year` | Numeric | Year the outlet was established |
| `Outlet_Size` | Categorical | Outlet size (Small, Medium, High) |
| `Outlet_Location_Type` | Categorical | City tier of the outlet (Tier 1–3) |
| `Outlet_Type` | Categorical | Grocery store or supermarket type |
| `Item_Outlet_Sales` | Numeric | Sales of the product at the outlet (target variable) |

### Data Quality

| Column | Missing Values | Share of Records |
|---|---|---|
| `Item_Weight` | 1,463 | 17.2% |
| `Outlet_Size` | 2,410 | 28.3% |

All other columns are complete.

## Notebook Walkthrough

| Step | Operation | Purpose |
|---|---|---|
| 1 | `import pandas as pd` | Import the library |
| 2 | `pd.__version__` | Confirm the installed version |
| 3 | `pd.read_csv()` | Load the dataset into a DataFrame |
| 4 | `data.head(3)` | Preview the first records |
| 5 | `data.shape` | Return the number of rows and columns |
| 6 | `data.columns` | List column names |
| 7 | `data.dtypes` | Inspect column data types |
| 8 | `data.isna().sum()` | Count missing values per column |
| 9 | `data.describe()` | Produce summary statistics for numeric columns |

## Getting Started

### Prerequisites

- Python 3.x
- pandas
- Jupyter Notebook or JupyterLab

### Installation

```bash
pip install pandas jupyter
```

### Usage

```bash
jupyter notebook "4. Pandas.ipynb"
```

Run the cells in order from top to bottom.

The notebook reads the dataset with a path relative to the project root (`Dataset/big_mart_sales.csv`), so launch Jupyter from the `Pandas_Trials/` directory.

## References

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [10 Minutes to Pandas](https://pandas.pydata.org/docs/user_guide/10min.html)
