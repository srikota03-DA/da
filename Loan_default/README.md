# Loan Default Analysis Dashboard (Power BI)

## Project Overview
This project analyzes loan default patterns using a structured dataset and an interactive Power BI dashboard. The objective is to identify key risk factors and provide actionable insights to help financial institutions make data-driven lending decisions.

---

## Problem Statement
Financial institutions face challenges in identifying high-risk borrowers. This dashboard helps:

- Detect patterns leading to loan defaults  
- Understand customer segmentation (income, credit history, etc.)  
- Evaluate risk across different borrower groups  
- Support data-driven loan approval decisions  

---

## Dataset
This dataset includes borrower-level financial and demographic information.

- File: `Loan_default.csv`  
- Size: **255,347 rows, 19 columns**  

> Note: The dataset is used for analytical and educational purposes. Original source attribution is unavailable.

---

## Tools & Technologies
- Power BI Desktop  
- Power Query (Data Cleaning & Transformation)  
- DAX (Data Analysis Expressions)  
- Excel / CSV  

---

##  Steps Followed
1. Imported dataset into Power BI  
2. Cleaned and transformed data using Power Query  
   - Handled missing values  
   - Performed data profiling  
3. Created calculated columns and measures using DAX  
4. Built interactive visuals and KPI cards  
5. Added slicers for dynamic filtering  
6. Designed dashboard for clear storytelling  
7. Published report  

---

## Key KPIs
- Total Loan Applications  
- Total Defaulted Loans  
- Default Rate (%)  
- Average Loan Amount  
- Average Borrower Income  
- Credit Risk Segmentation  

---

## Dashboard Features
- Interactive filters for customer segmentation  
- Loan default distribution analysis  
- Comparison of defaulters vs non-defaulters  
- Risk analysis based on income, loan amount, and credit history  
- KPI cards for quick insights  

---

## Key Insights
- High-risk borrowers are strongly correlated with lower income and poor credit history  
- Certain loan ranges show significantly higher default rates  
- Credit history is a key predictor of loan default behavior  
- Data-driven segmentation improves risk assessment  

---

## Business Impact
This dashboard enables financial institutions to:

- Reduce default rates  
- Improve credit risk assessment  
- Optimize loan approval strategies  
- Increase profitability through better risk management  

---

## Key DAX Measures
DAX
Total Loan Applications = COUNTROWS(Loan_default)

Total Defaulted Loans = 
CALCULATE(
    COUNTROWS(Loan_default),
    Loan_default[loan_status] = "Default"
)

Default Rate % = 
DIVIDE([Total Defaulted Loans], [Total Loan Applications], 0) * 100

Average Loan Amount =  AVERAGE(Loan_default[loan_amount])

## Default Rate %

This measure calculates the percentage of loans that resulted in default, helping evaluate overall portfolio risk.

## Dashboard Preview
![snap 1](https://github.com/user-attachments/assets/460248da-65cc-4998-a65e-7a1d171d6cd3)

## Conclusion

This project demonstrates how data visualization and analytics can solve real-world financial problems. By leveraging Power BI and DAX, the dashboard provides meaningful insights into loan default behavior and supports better decision-making.

## Author

Srinath Kota
Data Analyst | Power BI | SQL | Python
