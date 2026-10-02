# Power BI DAX Measures

```DAX
Total Revenue = SUM('IoT Financial'[Revenue])
Total Net Profit = SUM('IoT Financial'[Net_Profit])
Total Operating Cost = SUM('IoT Financial'[Operating_Cost])
Total EBITDA = SUM('IoT Financial'[EBITDA])
Total Cash Flow = SUM('IoT Financial'[Cash_Flow])
Transaction Count = DISTINCTCOUNT('IoT Financial'[Transaction_ID])
Average ROI = AVERAGE('IoT Financial'[ROI])
Average Gross Margin = AVERAGE('IoT Financial'[Gross_Margin])
Average System Uptime = AVERAGE('IoT Financial'[System_Uptime])
Average Automation Efficiency = AVERAGE('IoT Financial'[Automation_Efficiency])
Average Performance Score = AVERAGE('IoT Financial'[Performance_Score])
Average Compliance Score = AVERAGE('IoT Financial'[Compliance_Score])
Average Fraud Risk = AVERAGE('IoT Financial'[Fraud_Risk_Score])
Average Device Error Rate = AVERAGE('IoT Financial'[Device_Error_Rate])
Profit Margin % = DIVIDE([Total Net Profit], [Total Revenue], 0) * 100
Operating Cost Ratio % = DIVIDE([Total Operating Cost], [Total Revenue], 0) * 100
Excellent Status % =
DIVIDE(
    CALCULATE([Transaction Count], 'IoT Financial'[Financial_Status] = "Excellent"),
    [Transaction Count], 0
) * 100
High Fraud Risk Transactions =
CALCULATE([Transaction Count], 'IoT Financial'[Fraud_Risk_Score] >= 0.7)
```
