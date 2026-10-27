# Week 13: Inferential Statistics & Hypothesis Testing

This file covers inferential statistics concepts including correlation analysis, hypothesis testing principles, parametric testing (Z-test vs. T-test), confidence interval estimation, and categorical testing using the Chi-Square test of independence.

---

### Correlation, Causation & Hypothesis Testing

* Scatter plots do numerical variables ke relationship ki direction (positive, negative, ya no link) aur strength (tight clustering ya spread) dikhate hain.
* Pearson correlation coefficient ($r$) strictly $-1 \le r \le +1$ ke beech hota hai, jahan sign direction aur value strength denote karti hai.
* Correlation ka matlab direct causation nahi hota kyunki confounding factors (jaise season, age, ya time trend) variables ko saath me influence kar sakte hain.
* Null Hypothesis ($H_0$) default no-effect ya equality ($=$, $\le$, $\ge$) claim hota hai, jabki Alternative Hypothesis ($H_1$) real difference ya effect ($\ne$, $>$, $<$) ko represent karta hai.
* P-value wo probability hai ki $H_0$ true hone ke bawajood aise extreme results milein; agar $p \le \alpha$ (commonly $0.05$) ho toh $H_0$ ko reject karte hain, aur $p > \alpha$ par fail to reject hota hai.

---

### Parametric Testing: Z-Test vs. T-Test

* Large samples ($n \ge 30$) aur known population standard deviation ($\sigma$) ke case me Z-test use hota hai:
  $$Z = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt{n}}}$$
* Small samples ($n < 30$) aur unknown variance (sample $s$ use karke) ke liye Student's T-test use hota hai jisme degrees of freedom $df = n - 1$ lagti hai:
  $$T = \frac{\bar{x} - \mu}{\frac{s}{\sqrt{n}}}$$
* T-test ke teen main forms hote hain: One-sample (benchmark comparison), Independent two-sample (do alag groups), aur Paired samples (same cohort par pre/post measurements).

---

### Confidence Intervals & Chi-Square Testing

* Confidence Interval population parameter ($\mu$) ke around reasonable range provide karta hai: $\text{CI} = \bar{x} \pm \text{Margin of Error}$.
* Margin of error formula: $\text{ME} = Z \times \text{Standard Error} = Z \times \left(\frac{\sigma}{\sqrt{n}}\right)$.
* Sample size badhne par interval narrow aur precise hota hai, jabki variance ya confidence level badhne par interval wide ho jata hai.
* $95\%$ confidence level ka matlab hai ki repeated sampling par banaye gaye $95\%$ intervals true population mean ko capture karenge.
* Chi-Square Test of Independence ($\chi^2$) do categorical variables ke beech dependency check karta hai do-way contingency tables use karke.
* Expected frequency formula: $E = \frac{\text{Row Total} \times \text{Column Total}}{\text{Grand Total}}$.
* Test statistic: $\chi^2 = \sum \frac{(O - E)^2}{E}$ across degrees of freedom $df = (\text{Rows} - 1) \times (\text{Columns} - 1)$.
* Agar calculated $\chi^2 > \text{Critical } \chi^2$ ho at level $\alpha$, toh $H_0$ reject hota hai aur categories ke beech statistically significant dependency confirm hoti hai.
