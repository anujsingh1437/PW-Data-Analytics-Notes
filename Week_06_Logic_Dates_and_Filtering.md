# Week 6: Excel Logical Functions, Date/Time Math & Filtering Mechanics 📊

This file tracks the core concepts covered during Week 6 of my Data Analytics program at PW Skills. The focus this week was on automated decision-making using logical functions, understanding Excel's serial date architecture, and executing precise filtering workflows.

---

## 🧠 1. Logical Functions & Conditional Operations (Lect. 19)
Writing rules for automated decision-making across datasets[cite: 7]:
* **Logical Tests:** Questions returning strictly `TRUE` or `FALSE` using comparison operators (`=`, `>`, `<`, `>=`, `<=`, `<>`)[cite: 7].
* **`IF` Function Syntax:** `=IF(logical_test, value_if_true, value_if_false)`[cite: 7].
* **`IFS` Function:** Modern replacement for deep nested IFs. Evaluates multiple conditions left-to-right: `=IFS(test1, val1, test2, val2, ..., TRUE, fallback_val)`[cite: 7].
* **Conditional Aggregations:**
  * `=SUMIF(range, condition, [sum_range])`: Adds values matching a specific criteria[cite: 7].
  * `=AVERAGEIF(range, condition, [average_range])`: Calculates mean for matching rows[cite: 7].

---

## 📅 2. Date & Time Serial Architecture (Lect. 18)
Understanding underlying serial values and executing date arithmetic[cite: 8]:
* **Serial Storage:** Dates are whole integers counting days since Jan 1, 1900[cite: 8]. Times are decimal fractions of a 24-hour day (e.g., 0.5 = 12:00 PM)[cite: 8].
* **Date Parsing & Assembly:** 
  * Extraction: `=DAY()`, `=MONTH()`, `=YEAR()`, `=HOUR()`, `=MINUTE()`, `=SECOND()`[cite: 8].
  * Rebuilding: `=DATE(year, month, day)` and `=TIME(hour, minute, second)`[cite: 8].
* **Business Timeline Functions:**
  * `=DATEDIF(start_date, end_date, "Y"|"M"|"D")`: Calculates elapsed time gaps[cite: 8].
  * `=NETWORKDAYS(start, end, [holidays])`: Counts working days excluding weekends/holidays[cite: 8].
  * `=WORKDAY(start_date, days, [holidays])`: Returns future/past target work date[cite: 8].
  * `=EOMONTH(start_date, months)`: Finds the last day of a relative month[cite: 8].
  * `=WEEKDAY(date, 2)`: Returns day index (1 for Monday through 7 for Sunday)[cite: 8].

---

## 🔍 3. Data Filtering & Visible Aggregation (Lect. 17)
Managing focused dataset views safely[cite: 9]:
* **Filter Rule:** Temporarily hides non-matching rows without deleting underlying data (`Ctrl + Shift + L`)[cite: 9].
* **Data Types Support:** Offers dedicated filters for Text (`Contains`), Numbers (`Between`, `Top 10`), and Dates (`Last Month`)[cite: 9].
* **Aggregation Trap:** Standard `SUM()` includes hidden filtered rows. Always use `SUBTOTAL(109, range)` to aggregate only visible cells[cite: 9].

---
