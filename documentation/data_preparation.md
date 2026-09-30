# Data Preparation

## Revenue Data Preparation

The monthly reports contained revenue categories as separate columns. Power Query was used to:

- Standardize the revenue data structure.
- Unpivot revenue category columns.
- Convert the revenue categories into rows.
- Create a Source Month field to identify the reporting month.
- Remove unnecessary fields and maintain only relevant analysis columns.
- Consolidate revenue data from multiple monthly reports.

These transformations produced a standardized revenue dataset suitable for analysis in Power BI.

## Expense Data Preparation

Expense information was provided across different sections of the monthly reports. The medication and maintenance/office supplies data were combined into a consolidated expense dataset.

The following transformations were performed:
- Combined relevant expense data.
- Removed unnecessary supplier and invoice columns.
- Standardized expense descriptions.
- Created a consistent expense structure across reporting months.
- Added the reporting month to the expense records.

## Expense Categorization

A master expense category mapping was created to classify individual expense descriptions into standardized expense categories.
This allowed expenses with similar purposes to be grouped together for analysis.

Examples of expense categories include:
- Medical Supplies
- Medication
- Maintenance
- Office Supplies
- Transportation
- And Other Operating Expenses

The mapping approach improved consistency when analyzing expenses across different months.

## Monthly Consolidation
The transformed revenue and expense datasets were consolidated across the available reporting months.
This created two main analysis datasets:
- Revenue
- Expenses

The consolidated datasets were then loaded into Power BI for data modelling and financial analysis.

## Data Quality Considerations

During data preparation, inconsistencies were identified across some monthly reports, including differences in reporting periods and the structure of financial information. These issues were reviewed during the cleaning and transformation process to improve consistency and ensure that the resulting datasets were suitable for analysis.

## Final Output

The data preparation process resulted in cleaned and consolidated revenue and expense datasets that were used as the foundation for the Power BI data model and financial performance analysis.
