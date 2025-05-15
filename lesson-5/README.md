## Lesson 5  
**Topic:** Data Modeling Basics  
**Prerequisites:** Download customer.csv, product.csv, sales.csv  

1. What is a primary key in a table?  
2. Name the two types of table relationships in Power BI.  
3. How do you create a relationship between two tables in Power BI?  
4. What is a "star schema"?  
5. Which table is typically the fact table in a sales dataset?  
6. Link Sales.csv to Customers.csv using CustomerID (one-to-many).  
7. Why is ProductID in Sales.csv a foreign key?  
8. Fix a relationship error where ProductID has mismatched data types.  
9. Explain why a star schema improves performance.  
10. Add a new column TotalSales in Sales (Quantity * Price from Products).  
11. Optimize a model with circular relationships—how would you resolve it?  
12. Create a role-playing dimension for OrderDate and ShipDate.  
13. Handle a many-to-many relationship between Customers and Products.  
14. Use bidirectional filtering sparingly—when is it appropriate?  
15. Write DAX to enforce referential integrity if a CustomerID is deleted.  

```Sales```
| OrderID | CustomerID | ProductID | Quantity | OrderDate  |
|---------|------------|-----------|----------|------------|
| 1001    | 101        | 1         | 2        | 1/5/2023   |
| 1002    | 102        | 2         | 5        | 1/10/2023  |
| 1003    | 101        | 3         | 1        | 1/15/2023  |

```Products```
| ProductID | ProductName | Category     | Price |
|-----------|-------------|--------------|-------|
| 1         | Laptop      | Electronics  | 1200  |
| 2         | Mouse       | Accessories  | 25    |
| 3         | Keyboard    | Accessories  | 80    |

```Customer```
| CustomerID | Name    | Region |
|------------|---------|--------|
| 101        | Alice   | North  |
| 102        | Bob     | South  |
| 103        | Charlie | East   |

