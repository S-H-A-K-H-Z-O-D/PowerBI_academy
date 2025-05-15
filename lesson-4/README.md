## Lesson 4  
**Topic:** Data Transformation with Power Query (Part 2)  
**Prerequisites:** Download Customers.xlsx, Orders.csv  

1. What is the difference between "Merge" and "Append" in Power Query?  
2. How do you split a "Full Name" column into "First Name" and "Last Name"?  
3. What is "Pivot Columns" used for?  
4. How do you undo a step in Power Query?  
5. What is the purpose of "Reference" vs. "Duplicate" in queries?  
6. Merge Orders.csv and Customers.xlsx on CustID (inner join).  
7. Pivot the Product column to show total Quantity per product.  
8. Append two tables with identical columns (e.g., Orders_Jan.csv + Orders_Feb.csv).  
9. Use "Fill Down" to replace nulls in the Email column with the previous value.  
10. Extract the domain (e.g., "example.com") from the Email column.  
11. Write M-code to merge queries dynamically based on a parameter (e.g., JoinType = "Inner").  
12. Unpivot a table with columns like "Jan_Sales," "Feb_Sales" into a "Month" and "Sales" format.  
13. Handle errors in a custom column (e.g., division by zero) using try...otherwise.  
14. Create a function in Power Query to clean phone numbers (e.g., remove dashes).  
15. Optimize a query with 10+ steps—identify bottlenecks and simplify.  

```Orders```
| OrderID | CustID | Product  | Quantity |
|---------|--------|----------|----------|
| 1001    | 101    | Laptop   | 1        |
| 1002    | 102    | Mouse    | 3        |
| 1003    | 101    | Keyboard | 2        |
| 1004    | 103    | Monitor  | 1        |

```Customers```
| CustID | Name    | Email               |
|--------|---------|---------------------|
| 101    | Alice   | alice@example.com   |
| 102    | Bob     | bob@example.com     |
| 103    | Charlie | charlie@example.com |
