# Linear Regression Model — README

## Overview
This Excel workbook **Linear Regression Model.xlsx** shows a basic linear regression example done entirely in Excel using built-in functions (no charts in this file).

## Data
- Columns: `A1` = **Hour(X)**, `B1` = **Score(Y)**.  
- Sample observations are in `A2:A7` and `B2:B7` (with corresponding Y values).

## Calculations / Formulas (Sheet1)
- **Slope**: cell `E12` contains `=SLOPE(B2:B6, A2:A6)` (slope `m` computed from rows 2–6).  
- **Intercept**: cell `E11` contains `=INTERCEPT(B2:B6, A2:A6)` (intercept `c` from rows 2–6).  
- **Forecast**: cell `B9` contains `=FORECAST.LINEAR(A7, B2:B6, A2:A6)` (predicts Y at X = value in `A7`).  
- The sheet also displays the linear equation layout `y = m x + c`.

## Summary Statistics (Sheet5)
- Contains descriptive stats for X and Y (mean, standard error, median, standard deviation, variance, skewness, kurtosis, range).


