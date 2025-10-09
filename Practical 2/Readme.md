# 🎓 Teachers Rating Dataset Analysis  

## 🧭 Objective  
The goal of this practical exercise is to analyze a **synthetic dataset of teachers’ ratings** using Python libraries such as **NumPy**, **pandas**, and **Matplotlib**.  
The analysis involves exploring statistical relationships, creating visualizations, and interpreting key factors that may influence teaching evaluations — such as **age**, **gender**, **beauty**, and **tenure**.

---

## 📊 Dataset Description  
This dataset contains information about **50 university instructors** and their teaching evaluation statistics.  
It is **synthetically generated** for the purpose of practicing data analysis, visualization, and statistical modeling.

| Column | Description |
|:--|:--|
| `teacher_id` | Unique identifier for each teacher (1–50) |
| `gender` | Gender of the teacher — either *Male* or *Female* |
| `age` | Age of the instructor (integer between 25 and 65) |
| `beauty` | Standardized attractiveness score (normally distributed, may contain outliers) |
| `students` | Number of students enrolled in the teacher’s class (10–200 range) |
| `eval` | Teaching evaluation score on a 2.0–5.0 scale |
| `tenure` | Indicates whether the instructor has tenure (*Yes* or *No*) |

---

## 🧩 Note  
This dataset is **entirely synthetic** — created for educational purposes to practice:  
- Data cleaning  
- Descriptive and inferential statistics  
- Visualization and feature exploration  
- Regression or correlation analysis  

There are **no real individuals** represented in this dataset.

---

## ⚙️ Tools Used  
- 🐍 **Python 3.x**  
- 🔢 **NumPy** – for numerical operations and random data generation  
- 🧮 **pandas** – for data manipulation and exploration  
- 📈 **Matplotlib / Seaborn** – for creating visualizations  
- 💻 **Jupyter Notebook / Google Colab** – for interactive analysis  

---

## Conclusion

1. **Duplicate Analysis**: Duplicates were identified using the `prof` column, and average and standard deviation of age were computed both for all observations and for a filtered dataset with one observation per instructor (up to 94 instructors).  
2. **Course Division Evaluation**: Bar charts show that instructors teaching Higher-division courses tend to receive slightly higher average teaching evaluations than those teaching Lower-division courses.  
3. **Age vs Evaluation**: Scatter plots indicate the relationship between instructor age and teaching evaluation scores, highlighting trends and variability.  
4. **Gender Differences**: Gender-differentiated scatter plots reveal minimal differences between male and female instructors in evaluation patterns.  
5. **Tenure Effects**: Scatter plots combining gender and tenure illustrate how experience and demographics may influence evaluation scores.

