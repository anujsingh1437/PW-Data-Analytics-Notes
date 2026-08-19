# Week 8: Advanced Data Validation, Conditional Formatting & What-If Analysis 📊

This file documents the core concepts covered during Week 8 of my Data Analytics program at PW Skills. The focus this week was on defensive data entry, dynamic visual rule-setting, and predictive business modeling.

---

## 🛡️ 1. Data Validation & Paste Special 
Enforcing data integrity and efficient cell transformations:
* **Data Validation:**
  * Setting hard input rules (Whole Numbers, Decimal limits, Date boundaries).
  * Creating dynamic Dropdown Lists to restrict manual user input.
  * Configuring custom Input Messages and Error Alerts (Stop, Warning, Information).
* **Paste Special Mechanics:**
  * Pasting Values only (stripping heavy formulas/formats).
  * `Transpose`: Flipping rows to columns and vice versa.
  * Direct arithmetic operations (Add, Subtract, Multiply) across cell ranges.
* **INDEX + MATCH Integration:** Matrix-level coordinate lookups across rows and columns.

---

## 🎨 2. Conditional Formatting 
Visualizing trends, thresholds, and outliers dynamically:
* **Preset Rules:** Highlight Cells Rules (Greater Than, Less Than, Duplicate Values, Text that Contains).
* **Visual Analyzers:** Data Bars (in-cell distribution), Color Scales (heatmaps), and Icon Sets (KPI indicators).
* **Custom Formula Rules:**
  * Writing custom logical formulas for conditional styling.
  * Using column-locking (`$A1`) to highlight entire rows based on a single condition.
  * Managing rule hierarchy using the Conditional Formatting Rules Manager.

---

## 🔮 3. What-If Analysis & Business Forecasting
Exploring different scenarios and reverse-calculating target metrics:
* **Goal Seek:**
  * **Set Cell:** The target output formula cell.
  * **To Value:** The desired target value.
  * **By Changing Cell:** The single input variable Excel adjusts to reach the goal.
* **Scenario Manager:** Creating and comparing different business cases (e.g., Best Case, Base Case, Worst Case) and generating summary reports.
* **Data Tables (Sensitivity Analysis):** Testing how changes in 1 or 2 variables simultaneously impact an end metric.
