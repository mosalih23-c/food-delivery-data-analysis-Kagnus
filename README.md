# Food Delivery Data Analysis – Week 1

## Project Overview

This project is part of the Kagnus Data Analytics Internship.

The objective of Week 1 is to understand, assess, and clean the Food Delivery dataset while preserving the original raw data.

## Dataset Information

- **Dataset:** Food Delivery Dataset
- **Rows:** 45,584
- **Columns:** 20
- **Format:** CSV
- **Source:** Kagnus Internship Dataset

## Week 1 Tasks

1. Dataset Inspection
2. Data Quality Assessment
3. Data Cleaning
4. Cleaning Documentation
5. Export and Verification

## Data Quality Assessment

The following checks were performed:

- Missing Values
- Duplicate Records
- Data Types
- Inconsistent Categories
- Potential Outliers using the IQR method

## Data Cleaning Summary

- Missing values in seven columns were handled using Median or Mode imputation.
- The 1,731 missing values in `Time_Orderd` were retained.
- No duplicate rows or duplicate IDs were found.
- `Order_Date` was converted from object to datetime.
- No categorical formatting corrections were required.
- Potential outliers were assessed using IQR without automatically deleting records.
- The original dataset was preserved.

## Export and Verification

The cleaned dataset was exported to:

`data/processed/food_delivery_cleaned.csv`

Verification results:

- Original dataset shape: 45,584 × 20
- Exported dataset shape: 45,584 × 20
- Column names match: True
- Remaining missing values: 1,731 in `Time_Orderd`
- Duplicate rows: 0
- Duplicate IDs: 0

## Project Structure

```text
food-delivery-data-analysis/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   └── 01_data_understanding_and_cleaning.ipynb
├── docs/
│   └── cleaning_log.csv
├── README.md
└── requirements.txt
```

## Tools and Libraries

- Python 3.10
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## How to Run

1. Clone or download this repository.
2. Install the required libraries:

   `pip install -r requirements.txt`

3. Place the original dataset in `data/raw/`.
4. Open the notebook:

   `notebooks/01_data_understanding_and_cleaning.ipynb`

5. Run the notebook cells in order.

## Internship

**Program:** Kagnus Data Analytics Internship  
**Week:** 1 – Dataset Understanding and Cleaning