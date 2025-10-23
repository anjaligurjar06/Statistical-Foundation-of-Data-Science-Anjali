# 🎓 Practical 6 — Teachers’ Rating Dataset Statistical Analysis

This practical demonstrates the application of **probability** and **hypothesis testing** techniques using the **Teachers’ Rating Dataset**.  
It explores relationships between professors’ demographics and their teaching evaluation ratings through **t-tests**, **ANOVA**, **Chi-square**, and **Correlation** analysis.

---

## 🧭 Objective

The goal of this practical is to:
- Apply statistical hypothesis testing to real-world educational data.  
- Test differences and relationships between variables such as gender, age, beauty, and teaching evaluations.  
- Interpret results using **p-values** and **significance levels (α = 0.05)**.

---

## 📊 Dataset Description

The dataset, named **`teachers_rating_an.csv`**, contains demographic and professional details of university professors, along with their evaluation scores.

| Column | Description |
|:-------|:-------------|
| `prof` | Unique identifier or name of the professor |
| `age` | Age of the professor |
| `eval` | Overall teaching evaluation score (scale of 1–5) |
| `beauty` | Perceived attractiveness score of the professor |
| `rating` | Average teaching performance rating |
| `students` | Number of students who rated the professor |
| `gender` | Gender of the professor *(Male/Female)* |
| `tenure` | Indicates tenure status *(Yes/No)* |
| `division` | Type of course taught *(Lower or Upper division)* |

---

## 🧰 Tools & Libraries Used

| Library / Tool | Purpose |
|:----------------|:---------|
| **Python (v3.x)** | Core programming language |
| **pandas** | Data manipulation and loading |
| **NumPy** | Numerical operations |
| **SciPy** | Statistical tests (t-test, ANOVA, chi-square, correlation) |
| **Matplotlib / Seaborn** *(if used)* | Data visualization |
| **Jupyter Notebook / Google Colab** | Interactive environment for execution |

---

## 🧪 Statistical Tests Performed

| Test | Purpose | Hypothesis |
|:------|:----------|:------------|
| **Independent T-Test** | Compares teaching ratings between male and female professors. | H₀: Gender does **not** significantly affect evaluation ratings. |
| **One-Way ANOVA** | Tests whether beauty scores differ across age groups. | H₀: Mean beauty scores are equal across age groups. |
| **Chi-Square Test of Independence** | Examines relationship between gender and tenure. | H₀: Gender and tenure are **independent**. |
| **Pearson Correlation Test** | Measures relationship between beauty and evaluation scores. | H₀: No linear correlation between beauty and evaluation. |

---

## 📈 Results Summary

| Test | Statistic | p-value | Decision (α = 0.05) |
|:------|:-----------|:---------|:--------------------|
| T-Test | *t-statistic printed in output* | *p-value shown in notebook* | Reject/Fail to reject H₀ based on p-value |
| ANOVA | *F-statistic printed* | *p-value shown* | Determines if beauty varies by age group |
| Chi-Square | *χ² statistic printed* | *p-value shown* | Checks if gender and tenure are related |
| Correlation | *r-value printed* | *p-value shown* | Determines strength and significance of relationship |

---

