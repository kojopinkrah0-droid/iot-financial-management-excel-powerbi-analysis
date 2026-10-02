# Excel Analysis Guide

## 1. Import and prepare the data
Open `data/IoT_Financial_Management_Dataset.csv` in Excel and convert the full range to an Excel Table (Ctrl+T). Name it `tblIoTFinancial`.

The source audit found 8,900 records, 39 fields, no missing values and no duplicate rows.

## 2. Recommended KPI cells
Create an `Executive Dashboard` sheet and use:
- Transactions: `=COUNTA(tblIoTFinancial[Transaction_ID])`
- Total Revenue: `=SUM(tblIoTFinancial[Revenue])`
- Total Net Profit: `=SUM(tblIoTFinancial[Net_Profit])`
- Average ROI: `=AVERAGE(tblIoTFinancial[ROI])`
- Average Uptime: `=AVERAGE(tblIoTFinancial[System_Uptime])`
- Average Automation Efficiency: `=AVERAGE(tblIoTFinancial[Automation_Efficiency])`
- Average Performance: `=AVERAGE(tblIoTFinancial[Performance_Score])`
- Average Compliance: `=AVERAGE(tblIoTFinancial[Compliance_Score])`

## 3. PivotTables
Create PivotTables for:
1. Region — Revenue, Net Profit, ROI and Performance Score.
2. Department — Revenue, Net Profit, ROI and Automation Efficiency.
3. Financial Status — transaction count, Revenue, Net Profit and Performance Score.
4. Credit Risk Level — Fraud Risk Score, Compliance Score, Security Breach Attempts and Anomaly Score.

## 4. Excel charts
Add:
- Clustered column: Net Profit by Region
- Bar chart: Automation Efficiency by Department
- Doughnut/column: Transactions by Financial Status
- Scatter: Automation Efficiency vs Performance Score
- Scatter: Gross Margin vs ROI

## 5. Conditional formatting
Use green for Excellent, light green/amber for Good/Moderate and red for Poor. Apply color scales to Fraud Risk Score, Compliance Score, Device Error Rate and Performance Score.

## 6. Slicers
Add Region, Department, Financial Status and Credit Risk Level slicers to the PivotTables.
