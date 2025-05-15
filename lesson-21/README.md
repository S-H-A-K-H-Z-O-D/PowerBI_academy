# Lesson 21
**Topic:** HR Analytics Dashboard – Project Plan & Requirements
**Prerequisites:** All data is provided in HR\_Analytics.csv file


1. Project Objective 
To design and build a comprehensive HR Analytics Dashboard using Power 
BI, which helps HR managers and executives monitor employee performance, 
retention trends, department-level KPIs, and engagement levels using 
interactive visuals, DAX measures, Power Query transformation, and 
publishing to the Power BI Online Service. 

2. Dataset Details 
Table Name: Employee_Performance 
Columns: - Employment_id - Department - Age - Job Title - Hire_Date - Years_at_company - Education_level - Performance_Score - Monthly_Salary - Work_Hours_per_Week - Project_Handled - Overtime_Hours - Sick_Days - Remote_Work_Frequency - Team_Size - Training_Hours - Promotions - Employee_Satisfaction_Score - Resigned (Yes/No) 

3. Power Query Editor – Data Preparation Steps 
-- Rename Columns to follow proper casing (e.g., Employment ID, Work 
Hours per Week). 
-- Change Data Types: - Dates: Hire_Date - Numeric: Monthly_Salary, Age, Years_at_company, etc. - Text: Job Title, Department, etc. 
-- Remove Duplicates on Employment_id. 
-- Create Calculated Columns: - Tenure Category: Based on Years_at_company (e.g., 0-2 = New, 3-5 = 
Mid, 6+ = Veteran) - Overtime Category: IF Overtime_Hours > 10 THEN "High", ELSE "Low" 
-- Clean Null Values: Replace or remove rows depending on importance. 
-- Create Date Table: Mark as Date table, join with Hire_Date. 

4. Data Model – Relationships - Connect Date Table to Hire_Date (One-to-Many) - Create simple star schema, ensure no circular dependencies - Optionally: Create Lookup Tables for Department, Education_level, etc. 

5. DAX Measures (Key KPIs) 
-- Employee Count 
-- Resignation Rate   
-- Avg. Performance Score 
-- Avg. Monthly Salary 
-- Avg. Training Hours 
-- Avg. Employee Satisfaction 
-- Overtime Utilization 
-- Sick Days per Employee 
-- Remote Work Adoption Rate 
-- Promotion Rate 
-- Avg. Tenure (Years at Company) 

6. Report Pages and Visuals 
Page 1: Executive Summary - Card: Total Employees - Card: Resignation Rate - Card: Avg. Performance Score - Card: Avg. Monthly Salary - Line Chart: Resignation Rate over Time - Clustered Column Chart: Department-wise Satisfaction 
Page 2: Department Insights - Bar Chart: Employees per Department - Heatmap: Avg. Salary vs Performance per Department - Pie Chart: Education Level Distribution - KPI: Avg. Tenure by Department 
Page 3: Employee Engagement - Gauge: Employee Satisfaction - Donut Chart: Remote Work Frequency - Clustered Column Chart: Avg. Overtime by Job Title - Scatter Plot: Training Hours vs Performance Score 
Page 4: Retention & Promotions - Matrix: Promotions by Department & Education Level - Bar Chart: Sick Days vs Resigned Employees - Line Chart: Training Trend over Years - Card: Promotion Rate 
Page 5: Filters and Slicers - Slicers: Department, Job Title, Education Level, Remote Work Frequency, 
Tenure Category, Resigned (Yes/No)

7. Power BI Features to Apply 
Power BI Desktop: - DAX for KPIs - Custom tooltips - Drillthrough pages - Bookmarks for navigation - Conditional formatting - Sync slicers 
Power Query Editor: - Data cleaning, calculated columns - Merging lookup tables (if applicable) - Categorizing and grouping 
Design: - Use consistent color themes - Add icons for Job Titles, Department - Use grid layout - Add company logo, titles.

8. Publish and Share (Power BI Online Service) 
-- Create Workspace: HR Analytics Workspace 
-- Publish the report from Power BI Desktop 
-- Set up Scheduled Refresh 
-- Create App and publish for stakeholders 
-- Assign Roles & Permissions - HR Team: View access - Managers: Access to department-specific view (RLS if needed) 
-- Mobile View Optimization

9. Optional Advanced Features - Row-Level Security (RLS) for department managers - Paginated Report: Print-ready HR summary - Power Automate: Send alert if resignation rate exceeds threshold - Q&A visual: Enable natural language questions 

10. Versioning and Maintenance - Document every update in Power BI Online Service - Keep a backup of PBIX file - Log last refresh date and publish history - Monthly check for data quality issues
