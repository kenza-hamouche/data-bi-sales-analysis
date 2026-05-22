# Data BI Sales Analysis

## Project Overview

This project is a business data analysis project carried out using Python and data visualization tools.
The goal of the project was to explore sales data, clean and transform the dataset, analyze business performance, and generate insights through visualizations.

The project simulates a small real-world Data Analyst / BI workflow using sales data from an e-commerce environment.

---

# Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook
* Git & GitHub

---

# Dataset

The project uses two CSV files:

* `Sales-UTF8.csv`
* `States-UTF8.csv`

The dataset contains information about:

* sales
* profits
* customers
* products
* shipping
* regions
* discounts
* order dates

---

# Project Steps

## 1. Data Loading

The CSV files were imported into Python using Pandas.

```python
sales = pd.read_csv("../data/Sales-UTF8.csv", sep=";", engine="python")
```

---

## 2. Data Exploration

The dataset structure was explored using:

* `.head()`
* `.info()`
* `.columns`
* `.unique()`

This helped identify:

* column types
* business variables
* missing values
* numerical and categorical data

---

## 3. Data Cleaning & Transformation

Several transformations were applied:

* conversion of dates into datetime format
* creation of new columns
* cleaning and standardization of column names

Example:

```python
sales["Shipping Delay"] = (sales["Ship Date"] - sales["Order Date"]).dt.days
```

New variables created:

* `Order Year`
* `Order Month`
* `Shipping Delay`

---

# Business Analysis

Several business analyses were performed:

## Sales & Profit Analysis

* total sales
* total profit
* average shipping delay

## Category Analysis

* best-selling categories
* most profitable categories
* categories with negative profit

## Regional Analysis

* sales by region
* profit by region

## Customer Analysis

* top customers by sales

## Product Analysis

* most profitable products
* least profitable products

## Discount Impact

The project also analyzed the relationship between discounts and profitability.

Result:

> Higher discounts generally reduced average profit.

---

# Data Visualization

Several charts were created using Matplotlib:

* bar charts
* horizontal bar charts
* line charts
* temporal sales analysis

Examples:

* Total Sales by Category
* Total Profit by Category
* Monthly Sales by Year
* Average Profit by Discount Rate

---

# Key Insights

Some important findings from the analysis:

* Office Machines generated the highest sales.
* Telephones and Communication generated the highest profit.
* Higher discounts negatively impacted profitability.
* Sales varied depending on regions and periods of the year.
* Average shipping delay was around 16 days.

---

# Project Structure

```text
data-bi-sales-analysis/
│
├── data/
├── cleaned_data/
├── notebooks/
├── dashboard/
├── screenshots/
└── README.md
```

---

# Conclusion

This project helped me practice:

* data cleaning
* exploratory data analysis
* business intelligence concepts
* KPI analysis
* data visualization
* business-oriented thinking

It also helped me strengthen my skills in Python and data analysis tools in preparation for future Data Analyst / BI opportunities.
