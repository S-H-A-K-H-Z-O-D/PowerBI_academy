## Lesson 2  
**Topic:** Importing Data into Power BI  
**Prerequisites:** Download Sales_Data.csv file  

1. List three data sources Power BI can connect to.  
2. What is the first step to import data into Power BI Desktop?  
3. How do you refresh imported data in Power BI?  
4. What file formats can Power BI import directly? (Name two.)  
5. What does the "Navigator" window show after selecting a data source?  
6. Import Sales_Data.csv and load only the "Product" and "Price" columns.  
7. How would you change OrderDate to a date format during import?  
8. What is the difference between "Load" and "Transform Data" in the import dialog?  
9. Why might you see an error when connecting to a SQL database? (Name one reason.)  
10. How do you replace a data source after importing it?  
11. Write the M-code to import only rows where Quantity > 1.  
12. How would you change the data source if Sales_Data.csv changed?  
13. Troubleshoot: Your CSV import fails due to a "mixed data type" error—how do you fix it?  
14. Connect to a live SQL database with parameters (e.g., filter by year).  
15. How would you automate data imports using Power BI and Power Automate?

```Sales_Data```
| OrderID | Product  | Quantity | Price | OrderDate |
|---------|----------|----------|-------|-----------|
| 1001    | Laptop   | 2        | 1200  | 1/5/2023  |
| 1002    | Mouse    | 5        | 25    | 2/5/2023  |
| 1003    | Keyboard | 1        | 80    | 2/5/2023  |
| 1004    | Monitor  | 1        | 300   | 3/5/2023  |
| 1005    | Laptop   | 1        | 1200  | 3/5/2023  |
