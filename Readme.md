#  A/B Test Analysis & Experimentation Insights

## 📘 Overview
This project focuses on **A/B Testing and Experimentation Analysis** to evaluate the impact of design or campaign changes on user behavior and performance metrics.  
Using statistical hypothesis testing, we determine whether a **variant (B)** performs significantly better than the **control (A)** group.


## 🎯 Objective
To apply A/B testing methods and evaluate if observed differences between two groups are **statistically significant**, providing data-driven insights for decision-making.

Example Use Case:
> Analyzing two marketing campaign versions to see which achieves a higher click-through rate (CTR) or conversion rate.

## 🧭 Project Workflow
1. **Data Collection** – Load dataset containing campaign/group data.  
2. **Data Cleaning** – Handle missing values and ensure valid metrics.  
3. **Exploratory Data Analysis (EDA)** – Visualize and compare A vs. B distributions.  
4. **Hypothesis Formulation** –  
   - H₀: There is **no difference** between A and B groups.  
   - H₁: There **is a significant difference** between A and B groups.  
5. **Statistical Testing** – Perform t-test or Mann-Whitney U test based on data normality.  
6. **Result Interpretation** – Evaluate test statistics and p-values.  
7. **Conclusion & Business Insights** – Provide recommendations based on outcomes.

## 📊 Example Dataset
| Column | Description |
|---------|-------------|
| `Campaign Name` | Control or Experiment variant |
| `Date` | Test period |
| `Amount Spent` | Marketing spend |
| `Impressions` | Total ad impressions |
| `Clicks` | Number of user clicks |
| `Conversions` | Purchases or sign-ups |
| `CTR` | Click-through rate (Clicks / Impressions) |

## 🧮 Statistical Methods
- **Normality Check** → Shapiro-Wilk test  
- **Variance Check** → Levene’s test  
- **Significance Testing** →  
  - Independent t-test (parametric)  
  - Mann-Whitney U test (non-parametric)  

## 🧠 Tools & Libraries
- `pandas` – Data manipulation  
- `numpy` – Numerical analysis  
- `matplotlib`, `seaborn` – Visualization  
- `scipy.stats` – Statistical hypothesis testing  
- `jupyter` – Interactive notebook analysis



## ⚙️ Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/yourusername/ab-test-analysis.git
cd ab-test-analysis
pip install -r requirements.txt



### 👨‍💻 Author: Sanket Kumar  
📧 Email: sanketsv11@gmail.com  
🎓 MCA – Artificial Intelligence & Machine Learning  
💡 Data Science Enthusiast passionate about analytics, experimentation, and business optimization through data.

---
