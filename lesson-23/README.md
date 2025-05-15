# Lesson 23

**Topic:** Power BI Final Dashboard Project – Car Sales Dashboard Requirements
=============================================================
Objective:
Design and build a fully interactive and professional Power BI Dashboard to analyze the performance of car sales based on the provided dataset. This project should demonstrate mastery of Power BI Desktop features, including data modeling, transformation, DAX, and dashboard design.

1. Key Performance Indicators (KPIs)
- Total Sales Revenue (SUM of sellingprice)
- Total Cars Sold (COUNT of VIN)
- Average Selling Price
- Average Car Condition
- Average Odometer Reading
- % Difference: Selling Price vs MMR = (sellingprice - mmr) / mmr

2. Advanced DAX Measures
- % Above MMR Price – number of cars sold above MMR
- Avg Selling Price by Make
- Sales Trend by Month/Year using saledate
- Top 5 Car Brands by Sales Volume
- Avg Condition by Body Type
- Sales by Transmission Type
- Price Deviation from MMR (Variance)

3. Time Intelligence
- Extract: Year, Month Name, Quarter from saledate
- Monthly Sales Trend Visual
- Date Slicer to filter entire dashboard dynamically

4. Add interactivity using slicers:
- Make
- Model
- Year
- Body
- Transmission
- Color
- State
- Seller

 5. Visuals to Include
 
| Visual Type        | Description                                 |
|--------------------|---------------------------------------------|
| Line Chart         | Monthly/Quarterly Sales Trend               |
| Bar Chart          | Top Brands by Sales Volume                  |
| Pie / Donut Chart  | Distribution by Body or Transmission Type   |
| Table / Matrix     | Sales Summary by Make & Model               |
| Map                | Sales by State                              |
| KPI Tiles          | Display Summary KPIs                        |
| Decomposition Tree | Drill-down: Make > Model > Year             |
| Treemap            | Seller-wise Revenue Contribution            |

6. Interactivity
- Drill-through: Navigate from Make to specific Model
- Tooltips: Show condition, odometer, etc.
- Enable cross-filtering and cross-highlighting between visuals

7. Data Modeling & Transformations
- Clean missing values (filter out rows with missing make, model, sellingprice)
- Calculated Columns:
    - Sale Month (from saledate)
    - Price Category (Low, Medium, High based on sellingprice)
- Create calculated tables if necessary for ranking or comparisons

8. Export & Sharing Features
- Bookmarks for different report views (e.g., Brand View, Model View)
- Report Page Tooltips
- Page Navigation (if multiple pages)
- Professional formatting: titles, themes, tooltips, font consistency

9. Bonus (Optional)
- Create a What-If Parameter for MMR margin (e.g., ±5%, ±10%)
- Use RANKX to rank best-selling models
- DAX Classification: "Fair", "Overpriced", or "Underpriced" based on price vs MMR/



# Note: car_prices.csv file are shared


