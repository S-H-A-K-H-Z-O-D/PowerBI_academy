# Lesson 18
**Topic:** Visual Calculations  
**Prerequisites:** Download sales\_with\_geodata.csv file  

- Puzzle 1: Confusing Totals  
   - Visual: Table
   - Columns: Product, Sales, Quantity, Sales / Quantity (as a new column)
   - Problem: The total of Sales / Quantity doesn’t match the sum of individual rows.
   - Question: Why is the total different? How would you rewrite the DAX to get the correct total?

- Puzzle 2: Filtered vs. Unfiltered Totals  
  - Visual: Bar Chart
  - Values: Total Sales (explicit measure), Total Sales (All Categories)
  - Axis: Category
  - Task: Write two measures:
  - One for total sales per category.
  - One ignoring the axis filter (always total sales for all categories).
  - Bonus: Add a % of total column.

- Puzzle 3: Changing Context with Slicers  
   - Visual: Card
   - Measure: Total Sales
   - Task: Add a slicer for Country.
   - Question: Why does the card change when you select different countries?
   - Follow-Up: Add a second measure to ignore the slicer.

- Puzzle 4: Misleading Average
   - Visual: Table
   - Columns: Region, Average Sales per Order
   - Problem: You calculate Average Sales using:
   - Average Sales = [Total Sales] / [Total Orders]
   - But results are incorrect in visual.
   - Question: Why doesn’t this work as expected in a visual?

* **Puzzle 5: Highlight Top Product per Category**  
  * Visual: Matrix  
  * Rows: Category, Product  
  * Values: Total Sales  
  * Task: Add a visual-level filter to show only the top-selling product per category.

* **Puzzle 6: Unexpected Blank Values**  
  * Visual: Table  
  * Columns: Customer, Sales in France  
  * Measure: `Sales in France = CALCULATE(SUM(Sales[Sales]), Sales[Country] = "France")`  
  * Problem: Some customers have blank values even though they made purchases.  
  * Question: Why? How to fix it?

* **Puzzle 7: Time Intelligence Confusion**  
  * Visual: Line chart  
  * Axis: OrderDate (by Month)  
  * Values: Sales, Previous Month Sales  
  * Task: Add a line for previous month's sales.  
  * Challenge: Handle edge cases like first month of year or missing months.

* **Puzzle 8: Row-Level Calculation**  
  * Visual: Table  
  * Columns: Product, Quantity, Discount per Unit, Total Discount  
  * Measure: `Total Discount = SUMX(Sales, Sales[Quantity] * Sales[Discount per Unit])`  
  * Question: Why use SUMX() instead of just multiplying two columns?

* **Puzzle 9: Rank with Ties**  
  * Visual: Table  
  * Columns: City, Total Sales, Rank  
  * Challenge: Use RANKX() to handle ties correctly and allow descending/ascending logic.

* **Puzzle 10: Dynamic Titles and KPIs**  
  * Visual: Card and Title  
  * Task: Show a dynamic card title that changes based on slicer (e.g., selected country).  
  * Measure: `Title = "Sales for " & SELECTEDVALUE(Sales[Country], "All Countries")`