# Week 9: Data Cleaning, Visualizations & Dynamic Pivot Tables 📊

This file tracks the core concepts covered during Week 9 of my Data Analytics program at PW Skills. The focus this week was on preparing raw datasets, selecting optimal chart types, and building interactive summary reports using Pivot Tables, Slicers, and Timelines.

---

## 🧹 1. Data Cleaning & Preparation 
Techniques to standardize unrefined datasets before analysis:
* **Structural Cleaning:**
  * `=TRIM()` and `=CLEAN()` to eliminate leading/trailing whitespace and non-printable characters.
  * Text standardisation using `=UPPER()`, `=LOWER()`, and `=PROPER()`.
* **Deduplication & Blanks:**
  * Highlighting duplicates via Conditional Formatting before removing them through the Data tab.
  * Locating missing records using `Go To Special` -> `Blanks` to handle null entries safely.
* **Data Transformation:**
  * Parsing combined values via `Text to Columns` and pattern recognition using `Flash Fill`.
  * Resolving numbers stored as text and fixing inconsistent date formats.

---

## 📈 2. Core Visualizations & Chart Selection 
Converting numeric datasets into clear business graphics:
* **Chart Selection Principles:**
  * **Column / Bar Charts:** Best for discrete categorical comparisons (e.g., sales by department or region).
  * **Line Charts:** Used for continuous data over time to track trends and growth trajectories.
  * **Pie Charts:** Representing proportional shares of a 100% total (best kept to fewer slices).
* **Chart Elements:** Adding concise chart titles, configuring X/Y axes, setting clean data labels, and formatting legends.

---

## 🗂️ 3. Pivot Tables, Pivot Charts & Interactive Controls 
Aggregating large datasets without writing complex formulas:
* **Pivot Table Anatomy:** Distributing dataset attributes across **Rows, Columns, Values, and Filters** to summarize metrics dynamically.
* **Pivot Charts:** Connected visualization layer that updates alongside the underlying Pivot Table structure.
* **Interactive UI Controls:**
  * **Slicers:** Interactive visual buttons for filtering categorical dimensions (e.g., Region, Product Category).
  * **Timelines:** Specialized temporal slicers used to filter dashboards across years, quarters, and months.
* **Best Practices:** Ensuring source tables have zero blank header rows and refreshing data cache after source updates.

---
