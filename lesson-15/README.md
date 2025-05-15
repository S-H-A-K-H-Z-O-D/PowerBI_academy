# Lesson 15
**Topic:** Movies Analyses Dashboard with DAX  
**Prerequisites:** All data is provided in Movies.xlsx


1. Load Movies.xls into Power BI desktop

2. Remove or impute missing values in Budget and Box Office (e.g., replace with 0 or median) 

3. Ensure all columns are in a appropriate  format.  

4. Create a separate DATE table by using Release Date column, use Addcolumns, Calendarauto, filter functions and make sure a relationship exist in the data model view between two tables.

5. Create the following DAX measures and calculated columns to practice filter contexts, aggregations, and time intelligence.
- Create a calculated column called profit by using Budget and Box office column
- Create a calculated column to categorize movies by run time for segmentation. (Run Time < 90, Short Run Time > 90 and Run Time < 120, Medium Run Time > 120 , Long) Create following measures:
    - Total Box Office 
    - Average Budget 
    - Average Margin 
    - Total movies with Oscars 
    - Top Genre by Box Office 
    - Year-over-Year Box Office Growth 
    - Average Nominations per Director 


6. Visualization Requirements: Create an interactive dashboard with the following visuals to practice Power BI’s visualization features.
- Page 1: Overview Dashboard. Recommended Visuals: 
    - Card: Total Box Office, Profit Margin, Movies with Oscars. 
    - Bar Chart: Total Box Office by Genre (stacked by Certificate). 
    - Line Chart: Box Office trend by Release Year. 
    - Slicer: Filter by Country and Release Date (range). 
    - KPI: YoY Box Office Growth (target: >0%). 

- Page 2: Director Analysis. Recommended Visuals: 
    - Treemap: Budget by Director (size by Budget, color by Oscar Wins). 
    - Table: List Directors, Total Nominations, Total Oscars, Avg Nominations per Director. 
    - Slicer: Filter by Genre. 
    - Donut Chart: Run Time Category distribution for selected Director. 
    
- Page 3: Genre and Country Insights Recommended Visuals:
    - Matrix: Genre vs. Country with Total Box Office as values. 
    - Pie Chart: Share of Box Office by Certificate. 
    - Custom Visual: Word Cloud for Genre (requires marketplace visual).
    - Slicer: Filter by Run Time Category. 
    - Use conditional formatting in the matrix (e.g., color scale for Box Office).