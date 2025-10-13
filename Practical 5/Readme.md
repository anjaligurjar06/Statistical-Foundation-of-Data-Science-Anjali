# 🎓 Teachers Rating Dataset Analysis

## 🧭 Objective

The purpose of this practical is to apply probability and hypothesis testing concepts using the Teachers’ Rating Dataset. Students will calculate probabilities of evaluation scores within specific ranges and conduct a two-tailed Z-test to compare sample means with a known population mean.

---

## 📊 Dataset Description
The dataset named ratings contains details of university professors and their corresponding teaching evaluation ratings.
It includes both demographic and professional information related to each professor.

| Column       | Description                                                                |
| ------------ | -------------------------------------------------------------------------- |
| **prof**     | Unique identifier or name of the professor                                 |
| **age**      | Age of the professor                                                       |
| **eval**     | Overall teaching evaluation score (scale of 1–5)                           |
| **beauty**   | Numerical score representing the perceived attractiveness of the professor |
| **rating**   | Average teaching performance rating                                        |
| **students** | Number of students who rated the professor                                 |
| **gender**   | Gender of the professor (Male/Female)                                      |
| **tenure**   | Indicates whether the professor is tenured (Yes/No)                        |
| **division** | Type of course taught (Lower or Upper division)                            |

---

## 🧰 Tools & Libraries Used

| Tool/Library | Purpose |
|---------------|----------|
| **Python (v3.x)** | Programming environment for analysis |
| **pandas** | Data manipulation and statistical calculations |
| **NumPy** | Numerical operations and probability computations |
| **Matplotlib** | Data visualization and plotting |
| **Google Colab** | Environment for executing code and displaying results |

---

## 🧾 Results Summary
| Analysis                | Description                                                                                       |
| ----------------------- | ------------------------------------------------------------------------------------------------- |
| **P(eval > 4.5)**       | Probability of professors receiving evaluation scores greater than 4.5                            |
| **P(3.5 < eval < 4.2)** | Probability of professors having evaluation scores between 3.5 and 4.2                            |
| **Z-Test Result**       | Determines if the mean score of regional players significantly differs from the professional mean |
