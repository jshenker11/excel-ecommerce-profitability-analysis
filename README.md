# E-Commerce Sales & Profitability Analysis

**Excel | PivotTables | Business Analytics | Regression Analysis**

## Overview

This project analyzes historical e-commerce transactions to understand sales performance, product profitability, purchasing patterns, and relationships between transaction profit and customer attributes. It combines Excel formulas, PivotTables, a comparative chart, and regression analysis to explore practical business questions.

The workbook includes the original analysis sheets and a newly organized **Portfolio Overview** tab that summarizes the main findings. The underlying data covers **January 5–July 14, 2020**.

## Highlights

| Measure | Result |
|---|---:|
| Transaction records | 5,030 |
| Total recorded revenue | $688,795.34 |
| Total recorded profit | $84,242.53 |
| Average profit per Tuesday transaction | $18.66 |
| Profit from the four highest-volume brands | $61,705.03 |
| Total profit during the 6 a.m.–noon interval | $51,816.99 |

*These figures describe the supplied sample, not the broader e-commerce market.*

## Business Questions & Approach

1. **When is a transaction most profitable?** Used a PivotTable to compare mean profit by weekday. Tuesday had the highest average profit per transaction in this sample (**$18.66**).
2. **Which brands sell the most units?** Ranked brands by quantity sold. The top four were **PAPAISON (1,245)**, **Hestra (1,034)**, **Mongoose (597)**, and **All Weather Sport (460)** units.
3. **How much profit do high-volume brands generate?** Summarized the same brands by profit, totaling **$61,705.03**. High sales volume does not necessarily imply the highest profit per item.
4. **Which time window has the highest total profit?** Grouped transactions into time intervals; the **6 a.m.–noon** interval produced **$51,816.99** in recorded profit.
5. **How do customer age and customer ratings relate to profitability?** Reviewed Excel regression outputs and coefficient significance across three analyses. Findings are associative, not causal.

## Regression Analysis

The original workbook contains three ordinary least-squares regression outputs:

| Worksheet | Observations | Predictors shown in output | Reported R² |
|---|---:|---|---:|
| Task 5-6 | 5,030 | Customer age, customer rating | 0.2815 |
| Task 8-9 | 3,336 | Customer rating | 0.5367 |
| Task 10 | 2,279 | Customer rating | 0.8013 |

**Important interpretation:** These regressions use *different subsets of data*. The R² values should **not** be read as the performance of a model improving from 0.28 to 0.80 on the same test population. In addition, statistical association does not establish a causal effect of ratings or age on profit.

## Workbook Contents

Open [`ecommerce-sales-profitability-analysis.xlsx`](ecommerce-sales-profitability-analysis.xlsx) in desktop Excel.

| Worksheet | Contents |
|---|---|
| **Portfolio Overview** | New project introduction, summary metrics, major findings, and visual comparison |
| Data Dictionary | Column definitions |
| Transactions | Original transaction-level data and calculated fields |
| Task 1 | PivotTable of average weekday profit |
| Task 2 | PivotTable ranking brands by units sold |
| Task 3-4 | Profit summary and chart for top-selling brands |
| Task 5-6 | Regression with customer age and ratings |
| Task 7 | Profit by transaction time interval |
| Task 8-9 | Regression analysis on a subset of records |
| Task 10 | Additional regression output on a narrower subset |

The task-numbered tabs are retained from the original workbook to preserve the analysis and calculations. The `Portfolio Overview` tab was added for easier navigation and presentation.

## Tools & Skills

- Microsoft Excel and formula-based calculations
- PivotTables and category-level aggregations
- Revenue and profit analysis
- Data visualization and business reporting
- Linear regression, coefficient interpretation, and statistical significance
- Analytical limitations and sample comparability

## How to Explore

1. Download and open `ecommerce-sales-profitability-analysis.xlsx` in Microsoft Excel.
2. Select the **Portfolio Overview** tab to see the project summary and chart.
3. Use the **Transactions** and **Data Dictionary** tabs to inspect the underlying data.
4. Review the task-numbered tabs for the original PivotTables, regression results, and chart.

No separate packages, scripts, or installations are required.

## Limitations

- This is a historical transaction sample from 2020, not a live commercial dashboard.
- The workbook does not document independent validation of the underlying dataset's provenance or completeness.
- Total profit by time interval is influenced by transaction volume and should not be mistaken for average profitability per transaction.
- Regression outputs use different subsets, so their R² values are not directly comparable.
- Observed patterns in customer ratings and profit do not establish causality.

## Files

```text
excel-ecommerce-profitability-analysis/
├── README.md
└── ecommerce-sales-profitability-analysis.xlsx
```
