# Wine Dataset Analysis 🍷  
A complete exploratory data analysis and dimensionality-reduction practical performed in Jupyter Notebook using the **Wine dataset** from `sklearn.datasets`.

---

## 📌 Objectives  
This practical covers the following tasks:

1. Displaying **basic statistics** using `describe()`
2. Creating **boxplots** grouped by class labels
3. Plotting a **scatterplot** using two variables
4. visualizing **covariance matrix**
5. Performing **data scaling** using StandardScaler
6. Demonstrating **class separation using PCA**

---

## 📂 Dataset  
The Wine dataset consists of chemical analysis of wines from three different cultivars.  
It includes **13 numerical features** and a target label with **3 classes**.

---

## 🛠️ Technologies Used  
- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Jupyter Notebook  

---

## 📘 Steps Performed  

### ✔ 1. Basic Statistics  
Used `pandas.DataFrame.describe()` to display mean, std, min, max, and quartiles of each feature.

### ✔ 2. Boxplot by Output Class  
Created boxplots for each feature grouped by the wine class to observe distribution differences.

### ✔ 3. Scatterplot  
Plotted two numerical variables to visualize relationships and class-level separation.

### ✔ 4. Covariance Matrix  
Computed and visualized covariance using `df.cov()` and a heatmap via seaborn.

### ✔ 5. Data Scaling  
Standardized all variables using `StandardScaler()` to normalize feature ranges.

### ✔ 6. PCA for Better Class Separation  
Performed **Principal Component Analysis** and plotted PC1 vs PC2, showing clear class clustering.

---

## 📊 Visual Outputs  
The notebook contains:
- Statistical table  
- Boxplots  
- Scatterplots  
- Covariance heatmap  
- PCA scatterplot


