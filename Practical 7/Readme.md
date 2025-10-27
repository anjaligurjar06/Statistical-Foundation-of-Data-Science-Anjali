# 🎓 Teachers Rating Dataset Analysis

## 🧭 Objective
The objective of this practical is to perform **statistical analysis** on the **Teachers’ Rating Dataset** using various inferential techniques such as **Regression**, **ANOVA**, and **Correlation analysis**.  
The study investigates how factors like **Gender**, **Age**, and **Beauty** influence the **Teaching Evaluation Ratings** of university professors.

---

## 📊 Dataset Description
The dataset (`teachers_rating_an.csv`) contains information about professors, including their demographic characteristics and student evaluation scores.

| Column | Description |
|---------|-------------|
| **Prof** | Professor’s name or identifier |
| **Gender** | Gender of the professor (Male/Female) |
| **Tenure** | Tenure status of the professor (Yes/No) |
| **Beauty** | Beauty score of the professor (numeric) |
| **Rating** | Teaching evaluation rating (numeric) |
| **Students** | Number of students who rated the professor |
| **Age** | Age of the professor |
| **Division** | Course division (Lower/Upper) |

---

## 🧰 Tools & Libraries Used

| Library / Tool | Purpose |
|----------------|----------|
| **Python (v3.x)** | Core programming environment |
| **pandas** | Data loading and manipulation |
| **NumPy** | Numerical computations |
| **statsmodels** | Regression, T-test, and ANOVA models |
| **scipy** | Statistical testing and correlation |
| **matplotlib / seaborn** | Data visualization |
| **Jupyter Notebook / Google Colab** | Execution and visualization environment |

---

## 🧩 Experiments & Code Summary

### 🔹 Q1. Regression with T-test  
**Objective:** Check whether **gender affects teaching evaluation ratings.**

**Method:**  
Performed regression using `ols('Rating ~ C(Gender)')` and an independent **t-test** between male and female ratings.

**Result Interpretation:**  
- If p-value > 0.05 → Gender does **not** significantly affect evaluation scores.

---

### 🔹 Q2. Regression with ANOVA  
**Objective:** Determine whether **beauty scores differ by age group.**

**Method:**  
Applied **ANOVA (Analysis of Variance)** using `ols('Beauty ~ C(age_group)')`.

**Expected Output:**
## 🧾 Results Summary
- **Gender-based regression** revealed if male and female instructors receive different evaluations.  
- **ANOVA** determined if **beauty perceptions** vary significantly by **age**.  
- **Correlation analysis** identified the strength and direction of association between beauty and rating.  

All analyses used **T-tests, F-tests**, and **correlation coefficients** to ensure valid statistical conclusions.

---

## 🏁 Conclusion
This practical provided hands-on experience in:
- Applying **regression analysis** and interpreting coefficients.  
- Conducting **T-tests** and **ANOVA** for hypothesis testing.  
- Exploring **correlation** between continuous variables.  

The exercise improved understanding of **data-driven hypothesis testing**, **inferential statistics**, and how demographic factors may influence **teaching evaluations**.

---
