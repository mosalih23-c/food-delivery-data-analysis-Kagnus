# Food Delivery Data Analysis

## Project Overview

This project analyzes food delivery data to understand delivery duration patterns and identify operational factors associated with delivery performance.

The analysis focuses on exploring how road traffic, weather conditions, vehicle types, delivery distance, and multiple delivery assignments relate to delivery duration. The project also provides data-driven business recommendations to support delivery planning and operational decision-making.

## Objectives

- Understand and assess the quality of the dataset.
- Clean and prepare the data for analysis.
- Explore delivery duration patterns and operational factors.
- Visualize key findings using Python.
- Develop evidence-based business recommendations.

## Dataset

The dataset contains **45,584 delivery records** and **20 columns**, including:

- Delivery duration
- Delivery person age and ratings
- Restaurant and delivery location coordinates
- Order date and time information
- Weather conditions
- Road traffic density
- Vehicle condition
- Order and vehicle types
- Multiple deliveries
- Festival information
- City classification

## Project Structure

```text
food-delivery-data-analysis/
│
├── data/
│   ├── raw/
│   │   └── Food delivery Dataset.csv
│   └── processed/
│       └── food_delivery_cleaned.csv
│
├── notebooks/
│   ├── 01_data_understanding_and_cleaning.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   ├── 03_visualization_and_interpretation.ipynb
│   └── 04_final_findings_and_business_recommendations.ipynb
│
├── docs/
│   └── cleaning_log.csv
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- VS Code
- Git & GitHub

## Project Workflow

### Week 1 – Data Understanding & Cleaning

- Inspected the dataset structure and data types.
- Identified missing values and duplicate records.
- Examined categorical consistency.
- Investigated numerical outliers.
- Handled missing values using appropriate statistical methods.
- Documented cleaning decisions.
- Exported the cleaned dataset.

### Week 2 – Exploratory Data Analysis

- Analyzed delivery duration distribution.
- Compared delivery duration across traffic conditions.
- Examined weather-related differences.
- Analyzed vehicle types.
- Investigated delivery distance and duration.
- Examined multiple deliveries and ratings.
- Documented observations and analytical limitations.

### Week 3 – Visualization & Interpretation

Created five visualizations:

1. Delivery duration distribution.
2. Median delivery duration by road traffic density.
3. Average delivery duration by weather conditions.
4. Delivery distance versus delivery duration.
5. Delivery duration distribution by vehicle type.

Each visualization includes an interpretation of the observed patterns.

### Week 4 – Final Findings & Business Recommendations

- Consolidated the key analytical findings.
- Developed operational recommendations.
- Documented project limitations.
- Prepared the final conclusion.

## Key Findings

- Average delivery duration was **26.29 minutes**, with a median of 26 minutes.
- Orders under Jam traffic conditions averaged **31.18 minutes**, compared with **21.46 minutes** under Low traffic conditions.
- Cloudy weather deliveries averaged **28.92 minutes**, compared with **21.86 minutes** under Sunny conditions.
- Average delivery duration increased from **22.88 minutes** for 0 multiple deliveries to **47.82 minutes** for 3 multiple deliveries.
- Motorcycle deliveries averaged **27.61 minutes**, while Scooter deliveries averaged **24.48 minutes**.
- Delivery distance showed a positive correlation with delivery duration (**r = 0.321**).
- Delivery ratings showed a negative correlation with delivery duration (**r = -0.331**).

## Business Recommendations

1. **Traffic-Aware Delivery Planning:** Consider traffic conditions when planning delivery operations and estimating delivery times.
2. **Optimize Multiple-Order Assignments:** Review order batching practices to balance operational efficiency and customer waiting time.
3. **Improve Delivery Time Estimation:** Incorporate distance, traffic, and weather conditions into estimated delivery times.

## Limitations

- Missing values were handled using statistical imputation methods.
- Invalid restaurant coordinates were excluded from distance-related analysis.
- Outliers were retained to preserve data variability.
- Correlation does not establish causation.
- Delivery partner experience was not available in the dataset.
- Rating values include potential data quality issues.
- Some categories have small sample sizes.

## Conclusion

The analysis identified several operational factors associated with delivery duration, including traffic congestion, weather conditions, multiple delivery assignments, vehicle types, and delivery distance.

The findings suggest opportunities to improve delivery planning, order allocation, and delivery time estimation. However, the recommendations require further validation through operational testing before implementation.

This project demonstrates the application of data cleaning, exploratory data analysis, data visualization, and evidence-based business interpretation to a real-world operational dataset.

## How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/mosalih23-c/food-delivery-data-analysis.git
```

2. Navigate to the project folder:

```bash
cd food-delivery-data-analysis
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Open the notebooks using Jupyter Notebook or VS Code.

5. Run the notebooks in order, starting from Week 1.

## Author

Data Analytics Internship Project

