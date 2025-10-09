# 🎓 Teachers Rating Dataset Analysis  

## 🧭 Objective  
The goal of this practical exercise is to analyze a **synthetic dataset of teachers’ ratings** using Python libraries such as **NumPy**, **pandas**, **Matplotlib**, and **Seaborn**.  
The analysis focuses on exploring statistical relationships, visualizing patterns, and interpreting key factors that may influence teaching evaluations — including **age**, **gender**, **tenure**, **course division**, **beauty**, and **student numbers**.

## 📊 Dataset Description  
This dataset contains information about **120 instructors**, with some repeated observations, and includes both demographic and evaluation metrics.  
It is **synthetically generated** for practicing data analysis, visualization, and statistical interpretation.

### Columns

| Column | Description |
|:--|:--|
| `prof` | Unique identifier for each instructor (e.g., Prof_1, Prof_2) |
| `gender` | Gender of the instructor — either *Male* or *Female* |
| `age` | Age of the instructor (integer between 25 and 65) |
| `eval` | Teaching evaluation score on a 2.0–5.0 scale |
| `tenure` | Indicates whether the instructor has tenure (*Yes* or *No*) |
| `division` | Course level taught by the instructor — *Lower* or *Upper* division |
| `beauty` | Standardized attractiveness score (normally distributed, may contain outliers) |
| `rating` | Overall teaching rating (numeric score) |
| `students` | Number of students enrolled in the instructor’s classes (10–200 range) |

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

# Conclusion

1. **Data Type**: The teachers’ rating dataset is **cross-sectional**, as it captures multiple instructors’ data at a single point in time rather than over a period.  
2. **Students Statistics**: The number of students per instructor varies, with the dataset showing the calculated **mean, median, minimum, and maximum values**.  
3. **Descriptive Summary**: A descriptive statistics table provides an overview of central tendency, dispersion, and distribution for key numeric variables such as `age`, `eval`, `beauty`, and `students`.  
4. **Beauty Distribution**: The histogram of the `beauty` variable shows a roughly **normal distribution**, with most instructors clustered around the mean and a few outliers.  
5. **Gender Differences in Beauty**: Average beauty scores for male and female instructors are very similar, with comparable **means and standard deviations**, suggesting minimal difference by gender.  
6. **Tenure by Gender**: A slightly higher percentage of male instructors are tenured compared to females, but the difference is small; tenure status is **fairly balanced across genders**.
.

