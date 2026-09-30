# Data Preparation

#Revenue Data Preparation

The monthly reports contained revenue categories as separate columns. Power Query was used to:

Standardize the revenue data structure.
Unpivot revenue category columns.
Convert the revenue categories into rows.
Create a Source Month field to identify the reporting month.
Remove unnecessary fields and maintain only relevant analysis columns.
Consolidate revenue data from multiple monthly reports.

This transformation produced a standardized revenue dataset suitable for analysis in Power BI.

#Expense Data Preparation

Expense information was provided across different sections of the monthly reports. The medication and maintenance/office supplies data were combined into a consolidated expense dataset.

The following transformations were performed:
Combined relevant expense data.
Removed unnecessary supplier and invoice columns.
Standardized expense descriptions.
Created a consistent expense structure across reporting months.
Added the reporting month to the expense records.
