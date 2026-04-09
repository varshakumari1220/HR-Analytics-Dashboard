
📊 HR Analytics Dashboard (Power BI)

#Overview
This project is an interactive HR Analytics Dashboard built using Power BI to analyze employee data and understand attrition trends.
It helps organizations identify key factors behind employee turnover and make data-driven decisions.

---

#Key KPIs
-  Total Employees: 963  
-  Attrition Count: 133  
-  Attrition Rate: 13.8%  
-  Average Age: 37  
-  Average Salary: 6.3K  
-  Average Years at Company: 6.9  

---

#📊 Dashboard Insights
- Highest attrition observed in **26–35 age group**
- Employees with **Life Sciences education** show highest attrition
- **Salary below 5K** has maximum attrition
- **Laboratory Technician** role has highest employee turnover
- Male attrition is higher than female

---

#Tools & Technologies
- Power BI (Data Visualization)
- Excel (Data Source)
- DAX (Data Analysis Expressions)

---

#Key DAX Measures
```DAX
AttritionCount = 
CALCULATE(
    COUNTROWS(HR_Analytics),
    HR_Analytics[Attrition] = "Yes"
)

AttritionRate = 
DIVIDE(
    [AttritionCount],
    COUNTROWS(HR_Analytics)
)


