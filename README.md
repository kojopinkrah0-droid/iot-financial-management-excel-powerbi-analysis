# IoT Financial Management — Excel & Power BI Portfolio

A portfolio project analyzing **8,900 IoT-enabled financial transactions across 39 variables**. The project combines **Microsoft Excel** for data auditing, KPI analysis and summary reporting with **Power BI** for interactive financial, operational, automation, risk and compliance dashboards.

## Dataset Quality
- 8,900 records and 39 columns
- No missing values
- No duplicate records
- 5 regions and 6 departments

## Key Findings
- Total revenue: **4,667,647,698.83**
- Total net profit: **1,364,116,558.93**
- Average ROI: **18.56%**
- Average system uptime: **95.03%**
- Average automation efficiency: **74.41%**
- Average performance score: **90.45**
- **77.1%** of records are classified as Excellent financial status.
- South has the highest average net profit among regions, while Investment has the highest average net profit among departments.
- Automation efficiency shows a positive descriptive relationship with overall performance, while the dataset supports additional investigation of device errors, latency, fraud risk and compliance.

## Dashboard Design

### 1. Executive Financial Overview
Revenue, Net Profit, ROI, EBITDA, Cash Flow, Profit Margin, regional performance and department performance.

### 2. IoT Operations & Automation
System uptime, automation efficiency, device errors, response time, network latency and performance score.

### 3. Risk & Compliance
Fraud risk, credit risk, security breach attempts, anomaly score and compliance score.

### 4. Financial Drivers
ROI, gross margin, operating cost, net profit and cash-flow relationships.

## Portfolio Assets

- `excel/iot_financial_excel_analysis.xlsx` — Excel analysis workbook
- `powerbi/DAX_Measures.md` — reusable Power BI measures
- `powerbi/Dashboard_Build_Guide.md` — page-by-page dashboard instructions
- `data/` — source and summary datasets
- `images/` — portfolio visuals

## Suggested Power BI Model
Load `IoT_Financial_Management_Dataset.csv` as **IoT Financial**. For this single-table analytical dataset, a clean flat model is sufficient for the portfolio. Create the measures in `DAX_Measures.md` and use Region, Department, Financial Status and Credit Risk Level as key slicers.

## Skills Demonstrated
**Excel · Data Cleaning · KPI Analysis · Pivot-style Summaries · Financial Analysis · Power BI · Power Query · DAX · Data Modeling · IoT Analytics · Risk Analysis · Data Visualization · Dashboard Design**

## Note
The portfolio reports descriptive relationships in the supplied dataset; correlations or group differences should not be interpreted as causal effects.
