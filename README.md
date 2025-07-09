# 🧪 A/B Testing Analysis: Control vs Treatment Webpage

This project demonstrates a comprehensive A/B testing analysis using both **frequentist** and **Bayesian** statistical methods to evaluate the effectiveness of a new webpage design.

---

## 📂 Dataset Overview

We analyzed an A/B testing dataset simulating an online experiment where users were randomly assigned to either a:

- **Control group** → Old webpage
- **Treatment group** → New webpage

The objective was to determine if the **new page improves user conversion rate**.

---

## 🔍 Project Workflow

### 1. ✅ Data Quality Checks
- Verified group assignments and page views to ensure correct experiment setup.
- Identified and removed inconsistencies (e.g., users in treatment group seeing old pages).

### 2. 📊 Group Summary
- Checked the distribution of users across the control and treatment groups.
- Ensured fair splitting to avoid biased comparisons.

### 3. 📈 Conversion Rate Calculation
- Calculated conversion rates for each group.
- Visualized user conversions by group.

### 4. 🧪 Frequentist Hypothesis Testing
- Conducted a **Z-test for proportions** to determine statistical significance.
- Result: **p-value > 0.05** → No statistically significant difference.

### 5. 🧠 Bayesian Inference
- Modeled conversion rates using **Beta distributions**.
- Simulated posterior distributions and calculated:
  - Probability that **treatment > control**
  - 95% **credible intervals** for conversion rates

---

## 📊 Key Visualization

![Posterior Distributions of Conversion Rates](https://github.com/AdokshSuryawanshi/A-B-testing/blob/main/Screenshot%202025-07-09%20163738.png)

- **Green**: Treatment group  
- **Blue**: Control group  
- Dashed lines represent mean conversion rates  
- Bayesian probability that treatment outperforms control ≈ **70%**

---

## 🧠 Business Interpretation

> While traditional hypothesis testing did not show a significant difference, Bayesian analysis revealed a **70% probability** that the treatment improves conversion.

This result is **promising but not definitive** — suitable for:
- Further testing with larger sample size
- Segmented A/B testing for more targeted insights

Bayesian thinking supports decision-making under uncertainty by expressing **degrees of belief** rather than binary decisions.

---

## 🛠 Tools & Libraries

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- SciPy for hypothesis testing
- `scipy.stats.beta` for Bayesian sampling

---

## 💡 What I Learned

- Importance of data validation before statistical testing
- Trade-offs between frequentist and Bayesian interpretations
- How to communicate A/B test results for business decision-making
