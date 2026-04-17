# hr-analytics-powerbi
Interactive HR analytics dashboard in Power BI analyzing workforce trends, attrition, and salary insights.
# HR Analytics Dashboard — Power BI

An interactive HR analytics dashboard built from a 1,500-row 
employee dataset as part of a structured data analytics course.

## Dashboard overview

**KPI row:** Total Employees (1.5K) · Current Employees (1.2K) 
· Terminated (237) · Termination Rate (16%) · Total Salary (21M)

**Employee insights:** Gender distribution (donut) · Education 
breakdown · Job Satisfaction levels · Work-Life Balance scores

**Trend analysis:** Monthly salary trend · Monthly termination 
trend · Quarterly new hires vs terminations · Salary spread by 
employment type and years at company

## DAX measures built

- `Total Employees` — COUNT of all employee records  
- `Current Employees` — CALCULATE with Attrition = "No"  
- `Terminated Employees` — CALCULATE with Attrition = "Yes"  
- `Termination Rate` — DIVIDE(Terminated, Total)  
- `Total Salary` — SUM of MonthlyIncome  
- `Average Salary` — AVERAGEX for comparison visuals  

## Key design decisions

- Used **Average Salary** (not Total) for comparison visuals 
  to avoid misleading scale differences
- Cross-filtering enabled across all visuals
- KPIs at top → employee insights middle → trends at bottom
- Slicers: Gender · Department · Attrition

## Dataset

1,500 rows · columns include: EmployeeID, Gender, Education, 
JobSatisfaction, WorkLifeBalance, MonthlyIncome, YearsAtCompany,
TotalWorkingYears, EmploymentType, DateStart, DateDeparture, 
Attrition

## Screenshot

![Dashboard Preview](dashboard_screenshot.png)

## Tools

Power BI Desktop · DAX · Excel
