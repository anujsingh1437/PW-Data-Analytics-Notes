# Week 7: Advanced Logical Operators, Error Handling & Lookup Functions 📊

This file tracks the core concepts covered during Week 7 of my Data Analytics program at PW Skills. The focus this week was on compound logical decision-making, defensive error handling, and mastering data retrieval across vertical, horizontal, and two-way lookup engines.

---

## 🧠 1. Compound Logic & Error Handling 
Combining multiple logical conditions and preventing spreadsheet errors:
* **Compound Logical Operators:**
  * `=AND(test1, test2, ...)`: Returns `TRUE` strictly when all conditions are met.
  * `=OR(test1, test2, ...)`: Returns `TRUE` if at least one condition is satisfied.
  * `=NOT(test)`: Flips logical output (`TRUE` to `FALSE` and vice versa).
  * `=XOR(test1, test2)`: Exclusive OR; returns `TRUE` when exactly one condition is met.
* **Logic Nested in IF:** Used to evaluate multi-criteria rules (e.g., `=IF(AND(Score>=40, Attendance>=75%), "Pass", "Fail")`).
* **Cell Inspection (`IS` Functions):** `=ISBLANK()`, `=ISNUMBER()`, `=ISTEXT()`, and `=ISERROR()` to validate cell payloads before computing.
* **Defensive Error Handling:**
  * `=IFERROR(formula, fallback_value)`: Catches all formula crashes and replaces them with clean defaults.
  * `=IFNA()`: Catches specifically `#N/A` lookup misses.
* **`SWITCH` Function:** Evaluates a single target value against exact matching pairs: `=SWITCH(target, val1, res1, val2, res2, default)`.

---

## 🔍 2. Lookup & Reference Mastery 
Joining separate data tables and dynamically pulling attributes across worksheets:
* **Vertical Lookup (`VLOOKUP`):**
  * Syntax: `=VLOOKUP(lookup_value, table_array, col_index_num, FALSE)`.
  * Traps: Only looks to the right of the key column; column insertion breaks hardcoded index numbers.
* **Horizontal Lookup (`HLOOKUP`):**
  * Searches across the top row and pulls from designated row numbers below: `=HLOOKUP(value, table, row_index, FALSE)`.
* **Legacy `LOOKUP`:** Older approximate search tool requiring strict ascending sorted data.
* **Modern `XLOOKUP` (The Universal Engine):**
  * Syntax: `=XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found])`[cite: 12].
  * Advantages: Searches in any direction (left/right/up/down), defaults to exact match, eliminates column counts, handles missing keys gracefully without `#N/A`[cite: 12].
* **The `INDEX + MATCH` Duo:**
  * Syntax: `=INDEX(return_range, MATCH(lookup_value, lookup_range, 0))`[cite: 12].
  * Core Mechanics: `MATCH` identifies coordinate row index; `INDEX` extracts the value at that coordinate[cite: 12]. Highly resilient against structural column deletions/insertions[cite: 12].
