# Lesson 22
**Topic:** DAX practice  
**Prerequisites:** Download HR\_Analytics.csv file  

1. Top Performer Identification by Department
- Task: Write a measure that returns the Employment_id of the top performer (highest Performance_Score) in each department.
 2. Year-over-Year Promotion Growth
- Task: Create a measure that calculates the % increase or decrease in promotions compared to the previous year.
- Assume Hire_Date is used as a reference for the year.
3. Average Salary of Employees Who Resigned Within 2 Years
- Task: Calculate the average monthly salary of employees who resigned and had Years_at_company less than or equal to 2.
 4. Rank Employees by Satisfaction Score Within Their Department
- Task: Create a DAX measure or calculated column that ranks employees by Employee_Satisfaction_Score within their Department.
 5. Correlation Between Training Hours and Performance
- Task: Calculate the Pearson correlation coefficient between Training_Hours and Performance_Score.
 6. % of Employees Doing Remote Work Frequently
- Task: Write a measure that calculates the % of employees whose Remote_Work_Frequency is either "Weekly" or "Daily".
 7. Employees With Consistently High Performance Over Tenure
- Task: Identify employees with a Performance_Score of 4 or higher for every year at the company.
- You’ll need to assume or simulate a performance score per year using tenure approximation.
 8. Department-Wise Salary Budget Utilization
- Task: Calculate the total salary cost of each department and compare it against a predefined budget table using a RELATED or lookup mechanism.
9. Attrition Risk Index
- Task: Create a custom score to predict resignation risk using a formula like:
    ```IF  Employee_Satisfaction_Score < 3 && Overtime_Hours > 10 && Sick_Days > 5, "High",```
    ```IF(Employee_Satisfaction_Score < 4, "Medium", "Low"```
10. Identify Overworked but Unpromoted Employees
- Task: Count employees who:
    - Have worked more than 45 Work_Hours_per_Week
    - Have more than 5 Overtime_Hours
    - Have Promotions = 0


