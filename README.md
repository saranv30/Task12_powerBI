# Elevate Labs Data Analyst Internship  
**Task 12: Power BI – Data Transformation using Power Query**

## Task Summary
This task focused on real-world data preparation using **Power Query** in Microsoft Power BI Desktop.  
I imported, cleaned, transformed, and shaped the HR Analytics dataset to make it ready for visualization and analysis.

**Dataset Used**:  
IBM HR Analytics Employee Attrition & Performance  
(Source: Kaggle – https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)  
- ~1,470 employees  
- 35 columns (demographics, job details, salary, tenure, attrition, etc.)

## Main Transformations Performed in Power Query
1. Renamed columns for clarity (e.g., EmployeeNumber → EmployeeID)  
2. Removed unnecessary constant columns (EmployeeCount, Over18, StandardHours)  
3. Fixed data types (Age, MonthlyIncome, YearsAtCompany → Whole Number / Currency)  
4. Checked & handled any missing values (very few in this dataset)  
5. Created conditional columns:  
   - **AgeGroup**: Under 25 / 25-35 / 36-45 / 46+  
   - **SalaryBand**: Low / Medium / High / Very High  
   - **TenureBand**: New (0-2 yrs) / Mid (3-10 yrs) / Senior (10+ yrs)  
   - **AttritionFlag**: 1 if Attrition = "Yes", else 0  

All steps are visible in the **Applied Steps** pane in Power Query Editor.

## Visuals Built in Report View
Created 3 simple visuals to demonstrate the cleaned data:

1. **KPI Cards**  
   - Total Employees (Count Distinct EmployeeID)  
   - Attrition Count (Sum of AttritionFlag)  
   - Attrition Rate (%)  

2. **Clustered Column Chart**  
   - Department on X-Axis  
   - Attrition Count on Values  
   → Shows highest attrition in Sales and R&D departments  

3. **Donut Chart**  
   - Legend: TenureBand  
   - Values: Employee Count  
   → Displays distribution across tenure levels  

## Files Included
- **task12_transform.pbix** → Main Power BI file with transformations & visuals  
- **dashboard_export.pdf** → Exported report (static view of visuals)  
- **transformation_notes.txt** → Summary of steps and observations  
- **HR_Analytics.csv** → Original dataset  

## How to Open & Explore
1. Download the .pbix file  
2. Open in **Power BI Desktop** (free: https://powerbi.microsoft.com/desktop/)  
3. Check **Transform data** to see Power Query steps  
4. View **Report** page for the visuals  

