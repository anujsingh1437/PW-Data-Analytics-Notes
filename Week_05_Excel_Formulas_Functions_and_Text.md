# Week 5: Excel Data Types, Formulas, Functions & Text Manipulation 📊

This file tracks the core concepts covered during Week 5 of my Data Analytics program at PW Skills. The focus this week shifted to dataset organization, arithmetic operations, standard functions, and cleaning text data using formulas.

---

## 🗂️ 1. Data Types, Sorting & Filtering
Understanding data formats and organizing data efficiently:
* **Alignment Rules:** Text sits on the Left; Numbers and Dates sit on the Right by default[cite: 6].
* **Formatting Truth:** Formatting changes display/look, NOT the actual underlying value (as seen in the Formula Bar)[cite: 6].
* **Sorting:** Ordering datasets A-Z, Z-A, or Smallest-to-Largest[cite: 6]. Custom multi-level sorting (e.g., sort by Class first, then Marks)[cite: 6].
* **Filtering:** Hiding non-relevant rows dynamically without deleting data using `Ctrl + Shift + L`[cite: 6].

---

## 🧮 2. Basic Formulas & Arithmetic Functions
Writing calculations and leveraging core statistical functions:
* **Formula Syntax:** Every formula MUST start with an `=` sign (e.g., `=A1+B1`)[cite: 5].
* **Operators & BODMAS:** Uses `+`, `-`, `*` (multiply), `/` (divide), and `^` (caret for power)[cite: 5]. Follows BODMAS bracket precedence[cite: 5].
* **Core Functions:**
  * `=SUM(range)`: Totals numeric values (ignores text)[cite: 5].
  * `=AVERAGE(range)`: Returns the mean value[cite: 5].
  * `=MIN()` / `=MAX()`: Finds smallest and largest values[cite: 5].
  * `=COUNT()` vs `=COUNTA()`: `COUNT` counts numeric cells; `COUNTA` counts all non-empty cells[cite: 5].
* **Cell Locking:** Press `F4` to add `$` signs (Absolute Referencing, e.g., `$B$1`) when dragging formulas[cite: 5].
* **Common Errors:** `#DIV/0!` (divided by zero), `#VALUE!` (math done on text), `#NAME?` (typo in function name), `######` (column too narrow)[cite: 5].

---

## ✂️ 3. Text Functions & Data Cleaning
Cleaning messy strings, combining columns, and extracting sub-strings:
* **Combining Text:**
  * Using `&` operator: `=A2 & " " & B2`[cite: 4].
  * `=CONCAT()` or `=TEXTJOIN(separator, ignore_empty, range)`[cite: 4].
* **Extracting Substrings:**
  * `=LEFT(text, num_chars)` & `=RIGHT(text, num_chars)`[cite: 4].
  * `=MID(text, start_num, num_chars)`[cite: 4].
  * `=LEN(text)`: Counts characters[cite: 4].
* **Finding Position:** `=FIND()` (case-sensitive) or `=SEARCH()` (case-insensitive) to locate characters like `@` in emails[cite: 4].
* **Case & Cleaning:**
  * `=UPPER()`, `=LOWER()`, `=PROPER()` (Capitalizes first letters)[cite: 4].
  * `=TRIM()`: Removes extra stray spaces[cite: 4].
  * `=SUBSTITUTE()` & `=REPLACE()`: Swap specific characters or replace by positional index[cite: 4].
* **Format Conversion:** `=TEXT(value, "format")` to retain formatting; `=VALUE()` to convert text-stuck numbers[cite: 4].
* **No-Formula Tools:** `Flash Fill` (`Ctrl + E`) and `Text to Columns` on the Data tab[cite: 4].

---
