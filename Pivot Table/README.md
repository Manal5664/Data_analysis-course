# SalesData

This repository contains **SalesData.xlsx**, a sales workbook with raw
data, pivot analysis, and a dashboard.

------------------------------------------------------------------------

## 📑 Sheet Overview

### 1. `sales_data`

-   Contains the raw transactional records.
-   Columns:
    -   `Date`
    -   `Day`
    -   `Month`
    -   `Year`
    -   `Customer`
    -   `Customer_Age` / `Age_Group`
    -   `Customer_Gender`
    -   `Country`
    -   `State`
    -   `Product_Category`
    -   `Sub_Category`
    -   `Product`
    -   `Order_Quantity`
    -   `Unit_Cost`
    -   `Unit_Price`
    -   `Sales`
    -   **`Status`** ✅ (added column)

#### 🔹 Status Column Formula

The last column `Status` was created using the following formula:

``` excel
=IF(AND(M3=8,N3=45),"Proceed","Cancel")
```

-   Returns **"Proceed"** if:
    -   `Order_Quantity = 8`
    -   `Unit_Cost = 45`
-   Otherwise, returns **"Cancel"**.

👉 Recommended structured version (if converted to an Excel Table):

``` excel
=IF(AND([@Order_Quantity]=8,[@Unit_Cost]=45),"Proceed","Cancel")
```

------------------------------------------------------------------------

### 2. `Sheet3` (PivotTable)

-   Contains PivotTables for sales analysis.
-   Metrics included:
    -   **Sum of Sales**
    -   **Sum of Cost**
    -   **Sum of Profit**
-   Rows grouped by:
    -   `Age_Group`
    -   `Product`

------------------------------------------------------------------------

### 3. `Dash_Board`

-   Interactive dashboard for quick visualization.
-   Features:
    -   **Year slicer** (2011--2016)
    -   Bar chart comparing:
        -   **Sum of Sales**
        -   **Sum of Profit**
    -   Breakdown by `Age_Group`

------------------------------------------------------------------------
----------------------------------------------------------------

## 📝 Notes

-   `Sales = Order_Quantity * Unit_Price`\
-   `Cost = Order_Quantity * Unit_Cost`\
-   `Profit = Sales - Cost` (calculated in PivotTable or as a separate column)
------------------------------------------------------------------------

## ⚙️ Requirements

-   Microsoft Excel (recommended: 2016 or later).\
-   PivotTables and PivotCharts enabled.

------------------------------------------------------------------------

## ✅ Summary

This workbook demonstrates: - How to manage raw sales transactions.\
- Apply conditional formulas (`Status` column).\
- Build PivotTables for analysis.\
- Create an interactive Dashboard with slicers and charts.

------------------------------------------------------------------------
