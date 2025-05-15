# Lesson 16
**Topic:** Advanced Charting Techniques  
**Prerequisites:** Download Card\_data.csv file and disable Auto DateTime options by Options in Current File and create new DATE table by using Calendarauto and Format functions.   

- Total Card Limit by Card Brand and Card Type (Stacked Column Chart)  
  - X-axis: card\_brand (e.g., Visa, Mastercard, Amex)  
  - Y-axis: Sum of card\_limit  
  - Legend: card\_type (e.g., Credit, Debit, Prepaid)  
  - Tooltip: client\_id count (i.e., number of clients using this brand/type combo)  

- Drill Down into Monthly Trends (Drill Down Feature)  
  - Create a drill-down chart for analyzing card issues by time:  
    - Hierarchy: Year → Month (from account\_opened\_date)  
    - Values: Count of card\_number  
    - Chart type: Stacked Column Chart  
    - Enable drill down/up to move between years and months.  

- Top 10 Clients by Total Card Limit (Bar Chart)  
  - Axis: client\_id  
  - Value: Total card\_limit  
  - Filter: Top 10 clients  
  - Sort: Descending by total card limit  
  - Use a bar chart to clearly show top clients.  

- Client Drill-through Details  
  - Create a drill-through page showing all card details (e.g., card\_type, card\_brand, limit) for a selected client\_id when a user clicks from any chart.  
  - Add filters like card\_type or expire\_dates (Year).  

- Heatmap-style Matrix of Expiry Trends  
  - Rows: card\_brand  
  - Columns: Year of expire\_dates  
  - Values: Count of cards expiring  
  - Format as a matrix with conditional formatting to highlight peaks (red for more expiries).  

6. Create a dynamic slicer which will give options to select or to enter number and bar chart or column chart need to show only Top N (N should be selected by user in dynamic slicer) Card Brands according to their card limit. (column chart)  
   - X axis: Card Brand  
   - Y axis: Sum of Card Limit  

7. Download sales.csv file and disable Auto DateTime options by Options in Current File and create new DATE table by using Calendarauto and Format functions.  
   - Calculate Average number of days between Sales date and previous sales date for each customer  
     (ex:  
     last sales date 05.05.2025,  
     prev sales date 05.01.2025,  
     sales before prev sales date 04.21.2025  
     Answer: 7 (4 + 10) / 2)