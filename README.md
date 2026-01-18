# YOUTUBE SALES EXCEL-DASHBORAD
Most people think Excel is just for rows and columns. I decided to push it further.  I recently built this Adventure Works SalesDashboard to bridge the gap between complex data &amp;clear decision-making. By using advanced Pivot modeling and Neumorphic design principles,I turned over18,000 customer data points into a scannable, interactive experience.

<img width="1366" height="768" alt="Screenshot (119)" src="https://github.com/user-attachments/assets/9e2cd86e-0215-4699-beeb-e189e8c90b1e" />
<img width="1366" height="768" alt="Screenshot (117)" src="https://github.com/user-attachments/assets/b5422490-c163-4cc3-86d7-40fbbe7cb1e0" />

# 📊 Adventure Works Sales Analysis & Dashboard

An interactive, high-fidelity business intelligence solution built entirely in **Microsoft Excel**. This project transforms over **18,000+ rows** of raw transactional data into a dynamic, executive-level reporting system.

---

## 🚀 Project Highlights
* **Revenue Analyzed:** $307.1M
* **Profit Captured:** $126.3M
* **Customer Base:** 18,484 unique records
* **UI Style:** Modern Neumorphic (Soft UI) Dashboard Design

---

## 🔍 Key Business Insights

### 👥 Demographic Profile
* **The Silver Economy:** Discovered that the **50+ age demographic** is the primary profit driver, accounting for **50.2%** ($63.4M) of total profit.
* **Gender Balance:** Market performance is nearly equal, with females contributing 50.4% and males 49.6%.

### 🛍️ Product Intelligence
* **Power Categories:** Black-colored products are the market leader, generating **$39.2M** in profit.
* **Price Tiering:** High-end "Expensive" products dominate the profit share at **95.6%**, compared to just 4.4% for budget tiers.

### 📅 Time-Series Trends
* **Weekday Dominance:** Analysis revealed that **72% of profit** ($90.9M) occurs during the work week, suggesting higher B2B or routine consumer activity.
* **Seasonal Peaks:** Q2 stands out as the strongest period, contributing **31%** of annual performance.

---

## 🛠️ Technical Toolkit

- **Data Modeling:** Power Pivot & Advanced Pivot Tables.
- **Formulas:** Complex DAX-style measures, nested `IFERROR`, `VLOOKUP`, and `INDEX/MATCH`.
- **Visualization:** Dynamic Slicers, Custom Timeline filters, and Horizontal/Vertical Bar Charts.
- **UI/UX:** Created a custom Neumorphic interface using Excel shapes and shadow layering for an app-like feel.

---

## 📁 How to Use
1. **Open** the `Adventure_Works_Sales.xlsx` file.
2. **Navigate** to the `P&C Dashboard` or `Time Series Dashboard`.
3. **Interact** with the Slicers (Country/Year) to see the entire dashboard update in real-time.

---

## 📧 Contact & Connect
**[Your Name]** [Link to your LinkedIn Profile]




<H1> Calculation methods used throughout the workbook:<H1>
<H5>
  
1. <>Key Metric Calculations
   
The dashboard uses specific formulas to calculate performance metrics:
Total Revenue: Aggregated via a measure in the Data Model from the FactInternetSales table.
Distinct Counts: Used for counting unique items (e.g., DCountr or CustomerKey) across the dataset.


2.Data Model & DAX (Power Pivot)

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
