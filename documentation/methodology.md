# Methodology

## Data Model

- The Power BI model was designed using a dimensional modelling approach to support financial analysis and reporting.
- The model separates transactional financial data from descriptive dimension tables to improve organization, filtering, and analysis.

## Fact Tables
The model contains the following fact tables
- FactRevenue
- FactExpenses

These tables contain the financial transactions used for revenue
and expense analysis.

## Dimension Tables

The model contains the following dimension tables:

- Date
- Expense Category
- Revenue Category

The Date dimension supports time-based analysis, while the Expense and Revenue Category dimension provides a standardized way to analyze revenue and operating
expenses.

## Measures

Key DAX measures were created to evaluate hospital financial
performance, including:

- Total Revenue
- Total Expenses
- Operating Result
- Revenue Contribution %
- Expense Contribution %

These measures were used throughout the dashboard to answer the
defined business questions.

## DAX Approach

DAX functions including `CALCULATE`, `ALL`, `REMOVEFILTERS`, and
`ALLEXCEPT` were used where appropriate to control filter context
and calculate financial performance metrics.

The calculations were designed to allow financial metrics to respond
appropriately to selections such as reporting month, revenue source,
and expense category.

## Dashboard Analysis

The dashboard was designed to provide an overview of the hospital's
financial performance while allowing users to explore revenue,
expenses, and financial trends over time.

The analysis focuses on:

- Revenue performance
- Revenue source contribution
- Expense distribution
- Operating costs
- Operating result
- Financial performance over time
