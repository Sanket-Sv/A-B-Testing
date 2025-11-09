# Project Documentation: A/B Test Analysis

## 1. Introduction
A/B testing is a statistical experiment comparing two variants (A and B) to determine which performs better for a defined metric (e.g., CTR, conversion rate, revenue).  
This notebook walks through a full A/B testing pipeline from hypothesis design to statistical validation.

---

## 2. Objective
Evaluate whether differences between two experimental variants are statistically significant and actionable.

Example: Determine if a redesigned web banner improves click-through rates compared to the current one.

---

## 3. Data Preparation
- **Input:** Marketing campaign or product experiment dataset.  
- **Cleaning:** Remove missing/invalid entries.  
- **Feature Engineering:** Compute derived metrics (CTR, CVR, revenue per user, etc.).  
- **Grouping:** Split data into Control (A) and Variant (B).

---

## 4. Exploratory Data Analysis
Performed visual and descriptive analysis:
- Distribution plots for CTR and conversions  
- Boxplots and histograms for group comparisons  
- Mean/median analysis per group  
- Outlier detection and treatment  

---

## 5. Statistical Hypothesis Testing
- **Normality Test (Shapiro-Wilk):** Determines if sample data follow a normal distribution.  
- **Variance Test (Levene’s):** Tests equality of variances.  
- **T-Test / Mann-Whitney U Test:** Chooses appropriate test based on normality results.  

### Example Result:
| Test | p-value | Decision |
|------|----------|-----------|
| Shapiro (A) | 0.11 | Normal |
| Shapiro (B) | 0.09 | Normal |
| Levene | 0.28 | Equal Variance |
| T-Test | 0.03 | Reject H₀ → Significant Difference |

---

## 6. Interpretation
- **If p < 0.05** → Statistically significant difference; adopt new variant.  
- **If p ≥ 0.05** → No significant difference; retain existing version.  

---

## 7. Conclusion
The analysis provides evidence-based insights for business decisions.  
For example, a statistically significant uplift in CTR for Variant B implies improved user engagement.

---

## 8. Future Scope
- Include multi-variant (A/B/n) tests.  
- Automate hypothesis testing pipelines.  
- Apply Bayesian methods for more robust inference.  
- Integrate visual dashboards using Streamlit or Plotly.

---

### 📌 Author
**Sanket Kumar**  
🎓 MCA AIML | Data Science Enthusiast  
📫 [sanketsv11@gmail.com](mailto:sanketsv11@gmail.com)
