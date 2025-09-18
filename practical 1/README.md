Problem 1 — Mean, Median, Age-weighted Mean
📊 What was done

Created a synthetic dataset containing ID, Name, Age, Salary, and Department.

Introduced some NaN values in Age, Salary, and Department to simulate real-world missing data.

Computed:

Mean salary using df["Salary"].mean().

Median salary using df["Salary"].median().

Age-weighted mean salary, where employees’ salaries are weighted by their ages, to account for the idea that older employees may carry more weight in the analysis.

Problem 2 — Standardization & Outliers

First, the mean salary was calculated to represent the central tendency, and the standard deviation was calculated to measure how spread out the salaries are.


This expresses each salary in terms of how many standard deviations it is above or below the mean.

Interpretation:

Salaries with z ≈ 0 are close to the average.

Large positive z means much higher than average.

Large negative z means much lower than average.

To detect unusual cases, the rule |z| > 3 was applied. Such points are considered outliers.

In this dataset, no salaries crossed that threshold, meaning no extreme outliers were detected.

Problem 3 — Age Bins & Group Statistics (Summary)

Employees were grouped into age ranges: 18–25, 25–35, 35–45, 45–60.

For each group, the count, mean salary, and median salary were calculated.

Results showed:

Younger employees (18–25) had lower average salaries.

Salaries rose for the 25–35 and 35–45 groups.

The 45–60 group showed stable but mixed incomes.

Insight: Salary generally increases with age/experience, with the median being more reliable when outliers are present.


Problem 4 — NumPy Array Operations (Summary)

A 3×3 NumPy array was created.

Shape and size were checked to understand dimensions and total elements.

The transpose of the array was computed (rows → columns).

The array was also flattened into a one-dimensional sequence.

Insight: These operations are fundamental in NumPy for reshaping, preparing data for computations, and working with matrices in machine learning or statistical analysis.

 Goal
To implement statistical concepts step by step, understand their use in real-world data, and strengthen numerical computation skills using Python.

