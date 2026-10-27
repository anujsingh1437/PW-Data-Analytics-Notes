# Week 14: ANOVA, Probability Distributions & Linear Regression 📊

Compact summary notes covering multi-group mean comparisons, continuous and discrete probability distributions, and predictive modeling workflows.

---

### ANOVA (Analysis of Variance)

* 3 ya usse zyada groups ke means ko ek saath compare karne ke liye use hota hai bina Type-I error rate badhaye.
* Hypotheses setup:
  * Null Hypothesis ($H_0$): Sabhi groups ke means barabar hain ($\mu_1 = \mu_2 = \dots = \mu_k$).
  * Alternative Hypothesis ($H_1$): Kam se kam ek group ka mean alag hai.
* F-Statistic variance ka ratio measure karta hai:
  $$F = \frac{\text{Between-Group Variation}}{\text{Within-Group Variation}}$$
* Decision rule: Bada $F$-value aur $p \le 0.05$ hone par $H_0$ reject karte hain.
* ANOVA sirf ye batata hai ki difference maujood hai; kaunse specific pairs alag hain ye check karne ke liye Post-Hoc test lagana padta hai.

---

### Probability Distributions: PMF, PDF & CDF

* Random variables do tarah ke hote hain: Discrete (countable values, gaps) aur Continuous (unbroken range).
* Probability Mass Function (PMF): Discrete variables ke liye har exact point par probability batata hai, jahan sabhi outcomes ka sum 1 hota hai ($\sum P(X=x) = 1$).
* Probability Density Function (PDF): Continuous variables ke curve ke neeche ka area probability deta hai ($P(a \le X \le b) = \int_a^b f(x)dx$); kisi exact single point par probability zero hoti hai ($P(X=c) = 0$).
* Cumulative Distribution Function (CDF): Running total probability ($F(x) = P(X \le x)$) accumulate karta hai, jo 0 se 1 tak smoothly ya step-wise badhta hai aur kabhi decrease nahi hota.
* Standard distribution types
