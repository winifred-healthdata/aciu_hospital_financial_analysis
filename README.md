# ACIU Hospital Financial Performance Analysis

Financial performance analysis of ACIU Hospital using Excel, Power Query, and Power BI.

## Project Overview

This project analyzes the financial performance of a hospital using monthly revenue and expense data.

The objective was to transform raw hospital financial reports into a structured dataset, develop a dimensional data model, and build an interactive Power BI dashboard to evaluate revenue, expenses, profitability, and financial trends over time.

The project covers the complete workflow from raw data preparation to data modelling, DAX calculations, and dashboard development.

## Business Questions

The analysis was designed to answer key financial questions, including:

- What is the hospital's total revenue?
- What is the total cost of operation?
- What are the major sources of revenue?
- What percentage of total revenue does each revenue category contribute?
- What are the major expense categories?
- What percentage of total expenses does each category contribute?
- How do revenue and expenses change over time?
- Is the hospital operating at a profit or loss?
- What is the hospital's profit margin?

## Tools & Technologies

- Data Preparation: Microsoft Excel, Power Query
- Data Modelling: Power BI, dimensional modelling
- Analytics: DAX
- Visualization: Power BI

## Data Preparation

The raw monthly hospital reports were transformed using Power Query.

Key data preparation steps included:

- Standardizing the structure of monthly reports
- Unpivoting revenue category columns
- Consolidating revenue data across reporting periods
- Combining relevant expense data
- Standardizing expense descriptions
- Creating standardized expense categories
- Adding reporting month information
- Removing unnecessary fields
- Preparing consolidated revenue and expense datasets for analysis

Detailed documentation of the data preparation process is available in:

`documentation/data_preparation.md`

## Methodology

The analysis followed a structured workflow:

1. Review and audit the raw hospital financial reports.
2. Clean and transform the data using Power Query.
3. Consolidate revenue and expense data across reporting months.
4. Design a dimensional data model in Power BI.
5. Create DAX measures for financial performance analysis.
6. Develop interactive dashboards.
7. Analyze revenue, expenses, and overall financial performance.

The detailed methodology is documented in [`methodology.md`](documentation/methodology.md).

## Data Model

The Power BI model follows a dimensional modelling approach.

### Fact Tables

- FactRevenue
- FactExpenses

### Dimension Tables

- Date
- Expense Category
- Revenue Category

The model separates transactional financial data from descriptive dimension tables to support filtering, aggregation, and financial analysis.

## DAX & Financial Analysis

DAX measures were created to evaluate financial performance, including:

- Total Revenue
- Total Expenses
- Operating Result
- Revenue Contribution %
- Expense Contribution %

Functions including `CALCULATE`, `ALL`, `REMOVEFILTERS`, and `ALLEXCEPT` were used to control filter context and calculate financial performance metrics.

Detailed methodology is documented in:

`documentation/methodology.md`

## Dashboard

The Power BI dashboard provides an overview of financial performance and allows users to explore revenue, expenses, and profitability over time.

### Dashboard Overview

![Dashboard Overview](images/dashboard_overview.jpg)

### Detailed Analysis

![Detailed Analysis](images/detailed_analysis.jpg)

## Key Insights & Recommendations

### 1. High Revenue Concentration in Drugs
**Insight:** Drug-related revenue contributed ₦18.57 million, representing 84.93% of total recorded revenue.

**Recommendation:** Management could track drug sales separately from medications provided free of charge to better understand where the hospital's drug revenue comes from.

### 2. Salary and Medication Drive Expenditure

**Insight:** Salary and medication accounted for 54.44% and 32.16% of total expenses respectively. Combined, they represented 86.60% of recorded expenditure.

**Recommendation:** Management could closely monitor staffing and medication costs because changes in these two areas can significantly affect total expenditure.

### 3. Monthly Expenses Are Influenced by Purchase Timing

**Insight:** Monthly expenses varied considerably across the analysed period. Some months recorded substantially higher expenditure, partly because medications may be purchased in bulk and used over several subsequent months.

**Recommendation:** Management could consider medication purchase timing and inventory levels when reviewing monthly expenses rather than evaluating individual months in isolation.

### 3. Overall Financial Performance Was Slightly Negative

**Insight:** Total expenses of ₦22.37 million exceeded total revenue of ₦21.86 million, resulting in a loss of ₦512,865 and a profit margin of -2.3%.

**Recommendation:** Management could regularly monitor the relationship between revenue and expenses and investigate periods where expenditure exceeds revenue.

### 5. Financial Performance Varied Across Months

**Insight:** Monthly financial results varied considerably, ranging from a surplus of ₦852,450 in January to a loss of ₦867,850 in March.

**Recommendation:** Management could investigate the factors behind significant month-to-month changes in financial performance, particularly during months with unusually high expenses or lower revenue.

### 6. Laboratory Services Were the Second-Largest Revenue Source

**Insight:** Laboratory services generated ₦1.96 million, representing 8.96% of total recorded revenue and making it the second-largest revenue category.

**Recommendation:** Management could monitor laboratory utilization and revenue trends alongside patient activity to identify opportunities to strengthen this revenue stream.

### Data Model

![Power BI Data Model](images/data_model.png)

## Project Structure

```text
aciu_hospital_financial_analysis/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── documentation/
│   ├── business_questions.md
│   ├── data_preparation.md
│   └── methodology.md
│
├── images/
│   ├── dashboard_overview.jpg
│   ├── detailed_analysis.jpg
│   ├── data_model.png
│   └── README.md
│
├── power bi/
│
└── README.md
