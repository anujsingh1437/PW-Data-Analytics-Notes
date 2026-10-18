# Inferential Statistics & Hypothesis Testing Foundations 📊

Comprehensive reference notes covering relationship analysis, statistical testing frameworks, parametric comparisons, confidence boundaries, and categorical dependency tests.

---

## 1. Correlation & Hypothesis Testing Foundations

### Correlation & Scatter Plots
* **Scatter Plot:** Visualizes pairs of numeric variables to inspect relationship direction and clustering strength.
* **Directions:** Positive (both variables rise), Negative (one rises, other falls), or No Linear Link (random distribution).
* **Strength:** Proximity of points to an imaginary straight line reflects the tightness of the relationship.

### Pearson Correlation Coefficient ($r$)
* **Range:** Strictly bounded between $-1 \le r \le +1$.
* **Sign (+/-):** Dictates positive or negative direction.
* **Magnitude:** Proximity to $\pm 1$ indicates linear strength (e.g., $+0.9$ strong positive, $-0.7$ strong negative, $0$ no linear link).

### Correlation vs. Causation
* **Rule:** Correlation does not establish cause and effect.
* **Confounding Variables:** Unobserved factors (seasonality, demographics, time trends) often drive simultaneous movement across variables.

### Hypothesis Testing Structure
* **Null Hypothesis ($H_0$):** Default baseline stating no effect, difference, or relationship ($=$, $\le$, $\ge$).
* **Alternative Hypothesis ($H_1$ or $H_a$):** The operational research claim proposing a real difference ($\ne$, $>$, $<$).
* **P-Value & Significance Level ($\alpha$):**
  * $p$-value represents the probability of seeing data as extreme as observed assuming $H_0$ is true.
  * Standard threshold: $\alpha = 0.05$.
  * **Rule:** If $p \le \alpha$, reject $H_0$. If $p > \alpha$, fail to reject $H_0$ (insufficient evidence; never state $H_0$ is proven).

---

## 2. Parametric Testing: Z-Test vs. T-Test

### Decision Flow

```

```
              Population SD (σ) Known?
                     /        \
                   No          Yes
                  /              \
             Use T-Test      Sample Size (n) > 30?
                              /        \
                            No          Yes
                           /              \
                      Use T-Test       Use Z-Test

```

```

### Key Comparison

| Feature | T-Test | Z-Test |
| :--- | :--- | :--- |
| **Sample Size** | Small ($n < 30$) | Large ($n \ge 30$) |
| **Population SD ($\sigma$)** | Unknown (use sample $s$) | Known ($\sigma$) |
| **Test Distribution** | Student's $t$-distribution | Standard Normal ($Z$) |
| **Degrees of Freedom** | $df = n - 1$ | Not applicable |

### Formulas
* **Z-Test:**
  $$Z = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt{n}}}$$
* **T-Test:**
  $$T = \frac{\bar{x} - \mu}{\frac{s}{\sqrt{n}}}$$
* **Common T-Test Variants:** One-Sample (vs. target value), Independent Two-Sample (two separate groups), and Paired Samples (same group across two time points).

---

## 3. Confidence Intervals & Chi-Square Test

### Confidence Interval (CI)
Provides an estimated range of values likely to contain the unknown population parameter:
$$\text{CI} = \bar{x} \pm \text{Margin of Error (ME)}$$
$$\text{ME} = Z \times \text{Standard Error (SE)} = Z \times \left(\frac{\sigma}{\sqrt{n}}\right)$$

* **Width Behavior:** Larger sample sizes decrease standard error (narrower interval); higher confidence levels or higher variance increase interval width.
* **Interpretation:** A $95\%$ confidence level signifies that $95\%$ of similarly constructed intervals across repeated samplings will capture the true population mean.

### Chi-Square Test of Independence ($\chi^2$)
Evaluates counts across categorical variables within a **Contingency Table** to detect significant dependencies.

* **Expected Frequency ($E$):**
  $$E = \frac{\text{Row Total} \times \text{Column Total}}{\text{Grand Total}}$$
* **Chi-Square Statistic:**
  $$\chi^2 = \sum \frac{(O - E)^2}{E}$$
  *(where $O$ = Observed count, $E$ = Expected count)*
* **Degrees of Freedom ($df$):**
  $$df = (\text{Rows} - 1) \times (\text{Columns} - 1)$$
* **Decision:** If calculated $\chi^2 > \text{Critical } \chi^2$ from the table at level $\alpha$, reject $H_0$ to confirm a statistically significant association between the categories.

```
