# Week 12: Quartiles, Data Distributions, Skewness & Probability Foundations 📊

This file documents the core statistical concepts covered during Week 12 of my Data Analytics program at PW Skills. The curriculum covered positional statistics (Quartiles, Percentiles, IQR), data shape analysis (Histograms, Normal Distribution, Skewness), and fundamental probability theory.

---

## 📐 1. Quartiles, Percentiles & Outlier Detection 
Positional measures used to partition sorted distributions independently of extreme values:
* **Quartiles:** Partition sorted data into four equal 25% segments:
  * **$Q_1$ (25th Percentile):** 25% of data points fall below this threshold.
  * **$Q_2$ (50th Percentile):** The distribution median.
  * **$Q_3$ (75th Percentile):** 75% of observations fall below this value.
* **Percentiles vs Percentages:**
  * **Percentage:** An absolute score out of 100.
  * **Percentile:** Relative standing indicating the proportion of the population scoring below a given threshold.
* **Interquartile Range ($IQR$):**
  * $IQR = Q_3 - Q_1$: Captures the spread of the middle 50% of data.
  * Resilient against extreme values and used as the standard benchmark for identifying outliers ($1.5 \times IQR$ rule).

---

## 📊 2. Data Distributions, Histograms & Skewness
Analyzing data frequency, shapes, and asymmetry:
* **Histograms:** Visual representation grouping continuous numeric data into contiguous intervals called **bins**. Bar adjacency reflects scale continuity.
* **Normal Distribution:**
  * Symmetrical bell curve where $\text{Mean} = \text{Median} = \text{Mode}$ at the central peak.
  * **Empirical Rule (68-95-99.7):**
    * $68\%$ of data falls within $\mu \pm 1\sigma$
    * $95\%$ of data falls within $\mu \pm 2\sigma$
    * $99.7\%$ of data falls within $\mu \pm 3\sigma$
* **Skewness (Follow the Tail):**
  * **Right-Skewed (Positive):** Tail stretches toward higher values; $\text{Mode} < \text{Median} < \text{Mean}$ (e.g., income distributions, delivery runtimes).
  * **Left-Skewed (Negative):** Tail extends toward lower values; $\text{Mean} < \text{Median} < \text{Mode}$ (e.g., easy exam results, retirement ages).
  * In skewed distributions, the median provides a more representative measure of central tendency than the mean.

---

## 🎲 3. Probability Foundations & Decision Making
Quantifying likelihood to support data-informed business decisions:
* **Core Vocabulary:**
  * **Outcome:** A single possible result.
  * **Sample Space ($S$):** The complete set of all possible outcomes.
  * **Event ($E$):** Specific subset of outcomes under evaluation.
* **Theoretical Probability Formula:**
  $$\text{Probability} = \frac{\text{Number of Favorable Outcomes}}{\text{Total Possible Outcomes}}$$
* **Probability Boundaries:** Scaled strictly from $0$ (impossible event) to $1$ (certain event), with $0.5$ representing even odds.
* **Complementary Events:** $P(\text{Event}) + P(\text{Not Event}) = 1$.
* **Event Dependency:**
  * **Independent Events:** The occurrence of one event does not influence subsequent outcomes (e.g., coin tosses).
  * **Dependent Events:** Earlier outcomes alter the remaining sample space (e.g., sampling without replacement).
* **Analytics Applications:** Customer churn estimation, fraud detection thresholding, demand forecasting, and quality assurance inspection.

---
