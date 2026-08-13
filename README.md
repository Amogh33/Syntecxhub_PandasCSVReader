# Syntecxhub Project 2: Pandas CSV Reader & Basic Analysis

A complete interactive data exploration, statistics, and filtering dashboard built using Python, Pandas, and Streamlit. This project is submitted as part of the **Syntecxhub Data Science Internship (Week 1)**.

---

## 🌟 Features

### 1. 🔍 Interactive Data Inspector
- Upload files in **CSV** or **Excel (.xlsx)** formats.
- Previews the dataset by displaying `head` and `tail` rows, with a slider to control how many rows are visible.
- Displays dataset shape (rows & columns count), missing values percentage, and estimated memory usage.
- Shows column names along with their exact Pandas data types (dtypes).

### 2. 📈 Descriptive Summary Statistics
- Computes numeric summary metrics including mean, median, min, max, count, standard deviation, and percentiles.
- Focuses on unique counts, top occurring categories, and frequency for non-numeric/text columns.
- Offers interactive select boxes to display specific metric breakdowns.

### 3. 🎯 Data Slicing & Advanced Filtering
- Select specific columns of interest (column-based slicing).
- Apply conditional filters dynamically based on column type:
  - **Numeric**: filter by exact values, range (via sliders), greater than, or less than operators.
  - **Categorical/Strings**: filter using a text "contains" search or selecting specific categories via a multi-select dropdown.
- Tracks sample size changes in real-time as filters are adjusted.

### 4. 💾 Save & Export Data
- Export the filtered data subset back to a **CSV** file with custom separators (comma, semicolon, tab).
- Export to an **Excel** spreadsheet (.xlsx) with a customizable sheet name.
- Direct in-browser download triggers.

---

## 📂 Project Structure

```text
Syntecxhub_PandasCSVReader/
│
├── sample_data/
│   ├── coffee.csv            # Keith Galli warmup coffee dataset
│   └── sales_data.csv        # Realistic multi-type sales dataset
│
├── app.py                    # Streamlit web application (dashboard)
├── run_analysis.py           # Standalone Python script for sales data analysis
├── run_bios_analysis.py      # Standalone Python script for athlete biography analysis
├── pandas_analysis.ipynb     # Jupyter Notebook walkthrough
├── requirements.txt          # Package dependencies
├── .gitignore                # Git ignore file (excludes virtual envs & output folder)
└── README.md                 # Project documentation
```

---

## ⚙️ Installation & Setup

Ensure Python (3.9+) is installed. Since we are using Anaconda, all dependencies are already available.

### Run the Web Dashboard
1. Open PowerShell / Command Prompt.
2. Navigate to the project folder.
3. Run the Streamlit server:
   ```bash
   streamlit run app.py
   ```
4. The dashboard will automatically launch in your default web browser (usually at `http://localhost:8501`).

### Run the Standalone Scripts
You can execute the standalone analysis scripts directly from the terminal to run the analysis offline and output results to the `output/` directory:
- **Sales Analysis:**
  ```bash
  python run_analysis.py
  ```
- **Athlete Biography Analysis:**
  ```bash
  python run_bios_analysis.py
  ```

### Run the Jupyter Notebook
You can open `pandas_analysis.ipynb` in VS Code, Jupyter Notebook, or JupyterLab:
```bash
jupyter notebook pandas_analysis.ipynb
```
Select the Python 3 kernel and run all cells to verify standard Pandas operations.


