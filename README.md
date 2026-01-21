# Customer Data Cleaning & Preprocessing

## Overview
This project focuses on **cleaning and preprocessing customer data** using Python and pandas.
The goal is to prepare a raw dataset for **data analysis and machine learning tasks** by handling
missing values, duplicates, and inconsistent data types.

The project demonstrates best practices in **data quality checks, preprocessing, and exploratory validation**.

---

## Dataset Description
The dataset contains customer-level information, including:
- Customer identifiers
- Service-related attributes
- Billing and payment information
- Target variables for prediction (if applicable)

> Note: The `customerID` column is removed as it does not contribute to predictive modeling.

---

## Data Cleaning Steps

### 1. Initial Data Inspection
Before cleaning, the following checks are performed:
- Dataset shape
- Number of duplicate records
- Missing values per column

---

### 2. Column Removal
- `customerID` is dropped as it is not useful for prediction or analysis

---

### 3. Duplicate Handling
- Duplicate rows are identified and removed to prevent bias and redundancy

---

### 4. Data Type Correction
- `TotalCharges` is converted from string/object to numeric
- Invalid values are coerced to `NaN`

---

### 5. Missing Value Treatment
- Missing values in `TotalCharges` are filled using the **median**
- Median is chosen for robustness against outliers

---

### 6. Post-cleaning Validation
After cleaning, the dataset is re-evaluated to ensure:
- No duplicate records remain
- Missing values are handled appropriately
- Data is ready for downstream analysis or modeling

---

## Technologies Used
- Python
- pandas
- Jupyter Notebook

---

## How to Run
1. Clone the repository
2. Open the Jupyter Notebook
3. Run the data cleaning cell(s) in order

```bash
pip install pandas
jupyter notebook
