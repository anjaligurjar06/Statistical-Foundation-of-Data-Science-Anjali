# 🌼 K-Nearest Neighbors (KNN) Classifier — Iris Dataset  

---

## 🧭 Objective  
The goal of this practical is to implement the **K-Nearest Neighbors (KNN)** algorithm on the **Iris dataset** and classify iris flowers into their respective species.

This practical includes:
- Exploratory Data Analysis (EDA)  
- Feature scaling  
- Model training and evaluation  
- Confusion matrix & accuracy  
- Classification report  
- Error rate vs K plot  
- Finding the best K  
- Visualizing the final KNN decision boundary  

---

## 📊 Dataset Description  
The Iris dataset contains **150 samples** of iris flowers belonging to **3 species**:

- **Setosa**
- **Versicolor**
- **Virginica**

Each sample contains 4 features:

| Feature | Description |
|--------|-------------|
| Sepal Length (cm) | Length of the sepal |
| Sepal Width (cm) | Width of the sepal |
| Petal Length (cm) | Length of the petal |
| Petal Width (cm) | Width of the petal |
| Target | Species label (0, 1, 2) |

---

## 🧰 Tools & Libraries Used

| Library | Purpose |
|--------|---------|
| **pandas** | Data manipulation |
| **NumPy** | Numerical operations |
| **matplotlib** | Error plotting & visualization |
| **seaborn** | EDA plots |
| **scikit-learn** | KNN model, scaling, evaluation |

---

## ⚙️ Methodology

### 1️⃣ Data Loading & EDA
- Loaded the Iris dataset using `sklearn.datasets`.
- Converted it into a pandas DataFrame.
- Performed:
  - `head()`  
  - `describe()`  
  - `groupby('target')`  
- Verified feature distribution and class balance.

---

### 2️⃣ Feature Scaling  
KNN is distance-based, so data was standardized using:

```python
from sklearn.preprocessing import StandardScaler
scaler = StandardScaler()
X_scaled = scaler.fit_transform(X)
```

---

### 3️⃣ Train-Test Split  
Data was divided into **80% training** and **20% testing**:

```python
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X_scaled, y, test_size=0.2, random_state=42)
```

---

### 4️⃣ Training KNN Model  
A basic KNN classifier was trained with `k=5`:

```python
from sklearn.neighbors import KNeighborsClassifier
knn = KNeighborsClassifier(n_neighbors=5)
knn.fit(X_train, y_train)
```

---

### 5️⃣ Model Predictions  
Predictions made on test data:

```python
y_pred = knn.predict(X_test)
```

---

### 6️⃣ Model Evaluation  
Evaluated using accuracy, confusion matrix, and classification report.

#### ✔ Accuracy

```python
from sklearn.metrics import accuracy_score
accuracy_score(y_test, y_pred)
```

#### ✔ Confusion Matrix

```python
from sklearn.metrics import confusion_matrix
cm = confusion_matrix(y_test, y_pred)
```

#### ✔ Classification Report

```python
from sklearn.metrics import classification_report
print(classification_report(y_test, y_pred))
```

---

### 7️⃣ Error Rate vs K Plot  
To find the best value of **K**, error rate was calculated for values 1–40:

```python
error = []

for i in range(1, 41):
    knn = KNeighborsClassifier(n_neighbors=i)
    knn.fit(X_train, y_train)
    pred_i = knn.predict(X_test)
    error.append(np.mean(pred_i != y_test))
```

Plotted using Matplotlib to visually detect the optimal K.

---

### 8️⃣ Selecting the Best K  
Based on the error plot, the best K was chosen (usually between **3 to 6** for this dataset).  
The model was retrained using the optimal **K value**.

---

### 9️⃣ Final Visualization  
A decision boundary visualization was plotted using two selected features (e.g., petal length & petal width) to show how KNN classifies the dataset.

---

## ✅ Conclusion  

- KNN performed **very well** on the Iris dataset, achieving **high accuracy**.  
- The dataset is well-separated, so KNN is an appropriate model.  
- Feature scaling significantly improved performance as KNN depends on distance measures.  
- Error rate vs K plot helped determine the **optimal value of K**, improving the model’s generalization.  
- Visualizing the decision boundary demonstrated how KNN separates the three Iris species in feature space.



