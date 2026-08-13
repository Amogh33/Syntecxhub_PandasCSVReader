# Syntecxhub Project 2: Pandas CSV Reader & Basic Analysis

A comprehensive data exploration, statistics computation, filtering, and export walkthrough using Python and Pandas. This project is submitted as part of the **Syntecxhub Data Science Internship (Week 1)**.

---

## 🌟 Features

### 1. 🔍 Data Inspector
- Reads datasets (`CSV` format) into Pandas DataFrames.
- Previews dataset structure using `head()` and `tail()` rows.
- Displays dataset shape (rows and columns count), column data types (`dtypes`), and general metadata (`info()`).

### 2. 📈 Descriptive Summary Statistics
- Computes summary stats for numeric columns (mean, median, min, max, std dev, percentiles).
- Focuses on unique counts, top occurring categories, and frequency for non-numeric/text columns.
- Demonstrates manual calculations for specific attributes (like `mean()`, `median()`, `std()`) on individual features.

### 3. 🎯 Data Slicing & Advanced Filtering
- Slices datasets by selecting specific columns of interest.
- Slices rows by index ranges using `iloc`.
- Applies advanced conditional query filters:
  - Single condition numeric filtering (e.g., transactions where `Revenue > $1000`).
  - Multi-condition categorical filtering (e.g., Category is `Electronics` AND Region is `East`).

### 4. 💾 Save & Export Data
- Dynamically creates a dedicated folder for outputs.
- Exports filtered subsets to **CSV** format.
- Exports filtered subsets to **Excel** format (`.xlsx`) using the `openpyxl` engine with custom worksheet sheet names.

---

## 📂 Project Structure

This repository is kept bare-minimum and contains the following files:

```text
Syntecxhub_PandasCSVReader/
│
├── sample_data/
│   ├── coffee.csv            # Coffee sales warmup dataset
│   └── sales_data.csv        # Realistic multi-type retail sales dataset
│
├── pandas_analysis.ipynb     # Interactive Jupyter Notebook walkthrough (core code)
├── requirements.txt          # Python package dependencies
├── .gitignore                # Excludes virtual environments and the generated output folder
└── README.md                 # Project documentation

