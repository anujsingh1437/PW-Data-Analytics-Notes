# Week 11: Foundational Statistics, Central Tendency, Dispersion & Sampling 📊

This file marks the transition from spreadsheet engineering to foundational statistical analysis in my Data Analytics program at PW Skills. It covers data classification, measures of central tendency, variability quantification, and population sampling frameworks.

---

## 📌 1. Data Classification & Statistical Foundations
Understanding structural properties and analytical scopes of data:
* **Qualitative (Categorical) Data:**
  * **Nominal:** Discrete categories with no inherent ranking (e.g., Blood Group, Gender, City).
  * **Ordinal:** Categorical data carrying a logical rank/order, though mathematical intervals are undefined (e.g., Movie Ratings, Education Level, Exam Ranks).
* **Quantitative (Numerical) Data:**
  * **Discrete:** Countable whole units that cannot be subdivided (e.g., Number of students, Goals scored).
  * **Continuous:** Measurable values across a continuous scale with infinite subdivisions (e.g., Height, Weight, Transaction Revenue).
* **Data Architecture:** Structured schema-based data (rows/columns in RDBMS/Excel) vs Unstructured data (text logs, videos, social media streams).

---

## 🎯 2. Measures of Central Tendency & Outlier Dynamics 
Pinpointing the representative center of a distribution:
* **Mean:** Arithmetic average utilizing every data point. Highly sensitive to extreme values (outliers).
* **Median:** True midpoint of sorted observations. Extremely resilient to skewness and extreme outliers (ideal for income distributions).
* **Mode:** Most frequently occurring value. Applicable to both numeric and categorical attributes (e.g., most popular inventory size).
* **Outlier Sensitivity:** Outliers pull the mean away from the true center while leaving the median largely stable.

---

## 📐 3. Measures of Dispersion & Data Spread 
Quantifying variability and deviation around the mean:
* **Range:** Simplest measure (Maximum − Minimum). Fast to compute, but heavily distorted by single outliers.
* **Variance ($\sigma^2$):** Mean of squared deviations from the center, preventing positive and negative distances from canceling out.
* **Standard Deviation ($\sigma$):** Square root of variance, returning dispersion back into original data units for clear operational interpretation.
* **Quartiles & Interquartile Range (IQR):**
  * Divides sorted data into four equal partitions ($Q_1, Q_2/Median, Q_3$).
  * $IQR = Q_3 - Q_1$: Captures the middle 50% spread and powers Boxplot outlier boundaries.

---

## 🎲 4. Sampling Architectures 
Extracting representative subsets from large target populations:
* **Probability Sampling (Known, non-zero selection chance):**
  * **Simple Random:** Every unit has equal selection probability (e.g., lottery/ball draw).
  * **Systematic:** Choosing every $k$-th individual from a randomized baseline index.
  * **Stratified:** Segregating population into homogeneous strata (e.g., age tiers) and sampling proportionally from each.
  * **Cluster:** Partitioning population into representative heterogeneous clusters (e.g., geographic cities) and surveying selected full clusters.
* **Non-Probability Sampling (Subjective/Availability-based):**
  * **Convenience:** Selected purely on ease of physical/digital accessibility.
  * **Judgemental / Purposive:** Handpicked based on researcher domain expertise.
  * **Quota:** Convenience sampling constrained by demographic target caps.
  * **Snowball:** Existing participants recruit subsequent research units.
