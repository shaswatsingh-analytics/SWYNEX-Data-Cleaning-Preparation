# SWYNEX Technologies - Task 1
## Data Cleaning & Preparation

> A Python and Pandas-based data cleaning project completed as part of the Data Analyst Internship at SWYNEX Technologies.

---

## 📌 Overview

This project focuses on inspecting, cleaning, validating, and preparing the Netflix Movies and TV Shows dataset for further analysis.

The dataset was systematically checked for missing values, duplicates, incorrect data types, inconsistent formatting, and incorrectly placed values.

---

## 🎯 Problem Statement

Real-world datasets often contain missing values, inconsistent formatting, incorrect data types, and misplaced information.

The objective of this task was to identify and correct these data-quality issues while preserving the original information and avoiding unsupported assumptions.

---

## 📊 Dataset

**Dataset:** Netflix Movies and TV Shows  
**Original Size:** 8,807 rows × 12 columns

The dataset contains information about:

- Show ID
- Type
- Title
- Director
- Cast
- Country
- Date Added
- Release Year
- Rating
- Duration
- Listed In
- Description

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- Jupyter Notebook
- GitHub

---

## 🔍 Data Quality Checks

The following data-quality checks were performed:

- Missing values
- Exact duplicate records
- Duplicate `show_id` values
- Extra and repeated whitespace
- Incorrect data types
- Incorrectly placed values
- Duration formatting
- Rating formatting
- Categorical consistency
- Date formatting

---

## 🧹 Data Cleaning Performed

### Missing Values

Genuine missing values were retained because reliable replacement information was not available.

**Total missing cells:** 4,307

### Duplicate Records

- Exact duplicate rows: **0**
- Duplicate `show_id` values: **0**

### Whitespace Standardization

Leading, trailing, non-breaking, and repeated whitespace was standardized across relevant text columns.

**Whitespace issues identified:** 119 cells

### Incorrectly Placed Duration Values

Three movie duration values were incorrectly stored in the `rating` column.

These values were moved to the `duration` column, while the corresponding rating values were kept missing rather than creating unsupported information.

**Corrected records:** 3

### Data Type Correction

- `date_added` → datetime
- `release_year` → nullable integer (`Int64`)

### Date Standardization

The cleaned dataset was exported using the standardized date format:

`YYYY-MM-DD`

---

## 📈 Before vs After Validation

| Metric | Before Cleaning | After Cleaning |
|---|---:|---:|
| Rows | 8,807 | 8,807 |
| Columns | 12 | 12 |
| Exact Duplicate Rows | 0 | 0 |
| Duplicate `show_id` Values | 0 | 0 |
| Total Missing Cells | 4,307 | 4,307 |
| Duration-like Values in `rating` | 3 | 0 |

---

## 🔗 Project Files

| Resource | Description |
|---|---|
| 📓 [Cleaning Notebook](./notebooks/SWYNEX_Task_1_Data_Cleaning.ipynb) | Complete Python/Pandas cleaning workflow |
| 📂 [Cleaned Dataset](./data/netflix_titles_cleaned.csv) | Final validated dataset |
| 📄 [Raw Dataset](./data/netflix_titles.csv) | Original dataset used for the task |
| 📋 [Requirements](./requirements.txt) | Python dependency used in the project |

---

## 📁 Project Structure

```text
SWYNEX-Data-Cleaning-Preparation/
│
├── data/
│   ├── netflix_titles.csv
│   └── netflix_titles_cleaned.csv
│
├── notebooks/
│   └── SWYNEX_Task_1_Data_Cleaning.ipynb
└── requirements.txt

---

## ✅ Results & Conclusion

The Netflix Movies and TV Shows dataset was successfully inspected, cleaned, and validated using Python and Pandas.

The cleaning process addressed formatting issues, incorrect data types, and three incorrectly placed duration values.

The original dataset structure was preserved with **8,807 rows and 12 columns**.

No duplicate records were found, while genuine missing values were retained instead of being artificially filled.

The final cleaned dataset was exported as:

`netflix_titles_cleaned.csv`

---

## 👨‍💻 Internship & Author

**Internship:** Data Analyst Internship  
**Company:** SWYNEX Technologies  
**Task:** Task 1 - Data Cleaning & Preparation

**Author:** Shaswat Singh

**LinkedIn:** [Shaswat Singh](https://www.linkedin.com/in/shaswatsinghda27)

---

### ⭐ Project Repository

**SWYNEX Technologies - Data Cleaning & Preparation**

This repository contains the complete notebook, raw dataset, cleaned dataset, and project documentation.
