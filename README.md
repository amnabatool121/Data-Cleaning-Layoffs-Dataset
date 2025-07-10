# Data Cleaning – Layoffs Dataset

This project involves cleaning and preprocessing a raw dataset of global company layoffs using **T-SQL (SQL Server)**. The dataset includes information on companies, industries, layoff counts, funding, and dates. Cleaning the data prepares it for further analysis and visualization in tools like **Power BI**, **Excel**, or **Python**.


##  Project Description

The raw dataset, `layoffs_raw`, contains inconsistencies such as:
- Duplicate records
- Inconsistent text formatting (e.g., extra spaces, mixed casing)
- Special characters in names (e.g., "&" instead of "and")
- Null or missing values in key columns
- Unformatted date fields

This project uses SQL Server queries to clean, normalize, and format the data, making it ready for reliable business intelligence and data analysis.



 Features

- ✅ **Duplicate Removal**
  - Uses `ROW_NUMBER()` and CTE to identify and delete duplicate rows based on all attributes.

- ✅ **Text Standardization**
  - Trims whitespace
  - Converts text to lowercase for normalization
  - Capitalizes the first letter of words (title case)
  - Replaces special characters (e.g., `&` ➝ `and`)

- ✅ **Date Formatting**
  - Converts raw dates into clean `DD/MM/YYYY` or `YYYY-MM-DD` formats for consistency.

- ✅ **Null and Missing Value Handling**
  - Replaces string `'NULL'` values with `0` in numeric fields
  - Uses self-joins to fill missing values (e.g., industry names) based on company matches

- ✅ **Preview and Validation**
  - Final `SELECT` statement to confirm all cleaning steps were correctly applied.




Requirements

 Tools
- **SQL Server 2017 or later**
- **SQL Server Management Studio (SSMS)** or **Azure Data Studio**


