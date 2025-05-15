# Lesson 10
**Topic:** Advanced Filtering in DAX  
**Prerequisites:** Download Lesson 10.xlsx file.

1. What does FILTER(Sales, Sales\[Amount] > 1000) return?  
2. Write a measure High Sales that sums Amount where Amount > 1000 using FILTER.  
3. How does ALLEXCEPT(Sales, Sales\[Region]) differ from ALL(Sales)?  
4. Use SWITCH to categorize Amount:  
   ```"Low" if < 500  
   "Medium" if 500–1000  
   "High" if > 1000  ```
5. What is the purpose of ```ALLSELECTED```?  
6. Write a measure Regional Sales % showing each sale’s contribution to its region’s total (use ALLEXCEPT).  
7. Create a dynamic measure using SWITCH to toggle between SUM, AVERAGE, and COUNT of Amount.  
8. Use FILTER inside CALCULATE to exclude "Furniture" sales (Products\[Category] = "Furniture").  
9. Why might ALLSELECTED behave unexpectedly in a pivot table?  
10. Write a measure that calculates total sales and ignores filters from region  
11. Optimize this measure:  
    ```High Sales = CALCULATE(SUM(Sales\[Amount]), FILTER(Sales, Sales\[Amount] > 1000)) ``` 
    (Hint: Replace FILTER with a Boolean filter inside CALCULATE.)  
12. Write a measure Top 2 Products using TOPN and FILTER to show the highest-grossing products.  
13. Use ALLSELECTED with no parameters to respect slicers but ignore visual-level filters.  
14. Debug: A SWITCH measure returns incorrect values when fields are added to a matrix visual.  
15. Simulate a "reset filters" button using ALL in a measure.  

```Lesson 10```
| SaleID | ProductID | Amount | Region | SaleDate  |
|--------|-----------|--------|--------|-----------|
| 1      | P1        | 1200   | North  | 1/5/2023  |
| 2      | P2        | 800    | South  | 1/10/2023 |
| 3      | P1        | 1500   | North  | 1/15/2023 |
| 4      | P2        | 600    | East   | 1/20/2023 |
