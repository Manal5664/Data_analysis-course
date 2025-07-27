# Banking Dataset Analysis

This repository contains an Excel workbook used for a data analysis project.

## 📊 Excel File: Banking_Dataset_With_Mapping.xlsx

### Sheet 1: MainData
- Contains banking transaction records.
- Used for exploring customer behavior and transaction history.
Excel formulas used in this sheet:
  - `SUBTOTAL()`: To get total values on filtered data.
  - Applied **VLOOKUP** to fetch branch names from branchMapping using branch codes.
  - `LEFT()` and `RIGHT()`: To extract part of strings like branch codes.

### Sheet 2: branchMapping
- Maps branch codes to names.
- Excel formulas used in this sheet:
  - `SUMIF()`: For conditional summing.
  - `SUMIFS()`: For multi-condition summing.
  - `SUM()`: Add a list or range of values (used for overall totals) 
  
## 🎯 Goal
Practice Excel data analysis and mapping techniques as part of my course project.