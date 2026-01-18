# YOUTUBE SALES EXCEL-DASHBORAD
Most people think Excel is just for rows and columns. I decided to push it further.  I recently built this Adventure Works SalesDashboard to bridge the gap between complex data &amp;clear decision-making. By using advanced Pivot modeling and Neumorphic design principles,I turned over18,000 customer data points into a scannable, interactive experience.

<img width="1366" height="768" alt="Screenshot (119)" src="https://github.com/user-attachments/assets/9e2cd86e-0215-4699-beeb-e189e8c90b1e" />
<img width="1366" height="768" alt="Screenshot (117)" src="https://github.com/user-attachments/assets/b5422490-c163-4cc3-86d7-40fbbe7cb1e0" />

<H1> Calculation methods used throughout the workbook:<H1>
<H5>
1. <u> Key Metric Calculations </u>
The dashboard uses specific formulas to calculate performance metrics:
  
Total Revenue: Aggregated via a measure in the Data Model from the FactInternetSales table.
Distinct Counts: Used for counting unique items (e.g., DCountr or CustomerKey) across the dataset.

2.<U>Data Model & DAX (Power Pivot)</U>

The file heavily relies on an internal Data Model (Power Pivot) rather than just standard cell-based formulas. 
It contains:
 MdxScript:   Used for complex calculations and defining measures within the PivotTables.
 Relationship Formulas: Data is linked across multiple tables like Geography, Product, Customer, and Territory using keys (e.g., ProductKey, CustomerKey) to allow for multi-dimensional analysis.
 Aggregations: The system uses Sum and Count aggregations defined in the FactInternetSales metadata to generate dashboard values.

3. <U>Time-Based Analysis</U>

For the dashboard's timeline, the following data points are calculated:
Order Date & Month: Extracted and formatted from raw date strings to group revenue by time periods (e.g., Month_x0020_Number).
Age Groups: Calculated based on the BirthDate of customers to provide demographic breakdowns.

4.<U>Structural Formulas (Internal XML)</U>

The spreadsheet uses standard Excel structural elements in its worksheets:
Defined Names: Reference specific ranges for the dashboard visualizations.
PivotTable References: Many "formulas" on the visual dashboard sheet are likely GETPIVOTDATA functions or direct links to the Power Pivot model.
</H5>
