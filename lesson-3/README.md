## Lesson 3  
**Topic:** Data Transformation with Power Query (Part 1)  
**Prerequisites:** Download Customer_Orders.txt, Orders.txt  

1. What is the purpose of the "Applied Steps" pane in Power Query?  
2. How do you remove duplicate rows in Power Query?  
3. What does the "Filter" icon do in Power Query?  
4. How would you rename a column from "CustID" to "CustomerID"?  
5. What happens if you click "Close & Apply" in Power Query?  
6. Remove all rows where Quantity is less than 2.  
7. Split the OrderDate column into separate "Year," "Month," and "Day" columns.  
8. Replace all "Mouse" entries in the Product column with "Computer Mouse."  
9. Sort the table by OrderDate (newest first).  
10. How would you handle null values in the Price column?  
11. Write custom M-code to add a column calculating TotalSpent = Quantity * Price.  
12. Group the table by CustID to show total spending per customer.  
13. Fix inconsistent date formats (e.g., 01/10/2023 vs. 2023-01-10) in OrderDate.  
14. Create a conditional column: Label orders as "High Value" if Price > 100.  
15. Optimize the query to reduce refresh time (e.g., remove unused columns early).  

```Orders```
| CustID | Name    | OrderDate  | Product  | Quantity | Price |
|--------|---------|------------|----------|----------|-------|
| 101    | Alice   | 2023-01-10 | Laptop   | 1        | 1200  |
| 102    | Bob     | 2023-01-15 | Mouse    | 3        | 25    |
| 101    | Alice   | 2023-01-20 | Keyboard | 2        | 80    |
| 103    | Charlie | 2023-01-25 | Monitor  | 1        | 300   |


```Customer_orders```
| CustID | Name    | Email               |
|--------|---------|---------------------|
| 101    | Alice   | alice@example.com   |
| 102    | Bob     | bob@example.com     |
| 103    | Charlie | charlie@example.com |

