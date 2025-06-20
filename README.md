# 💓 Heart Disease Prediction using Machine Learning

This project predicts the presence of heart disease in patients using machine learning models such as K-Nearest Neighbors, Decision Tree, and Random Forest. Built with Python, the project demonstrates complete data analysis, feature engineering, model selection, and evaluation techniques.

---

## 📊 Dataset

- **Source:** UCI Machine Learning Repository
- **Rows:** 303
- **Features:** 14 (including age, sex, chest pain type, cholesterol, fasting blood sugar, etc.)
- **Target:** Binary (0 = No Heart Disease, 1 = Heart Disease)

---

## 🛠️ Technologies Used

- Python
- NumPy, Pandas
- Matplotlib, Seaborn
- Scikit-learn

---

## 🔍 Exploratory Data Analysis (EDA)

- Checked for null values (none found).
- Visualized class balance of the target variable.
- Plotted feature distributions using histograms.
- Correlation heatmap used to identify important features.

---

## ⚙️ Feature Engineering & Preprocessing

- Applied `get_dummies()` to convert categorical variables: `sex`, `cp`, `fbs`, `restecg`, `exang`, `slope`, `ca`, `thal`.
- Used `StandardScaler` to normalize continuous features: `age`, `trestbps`, `chol`, `thalach`, `oldpeak`.

---

## 🔮 Machine Learning Models

### ✅ 1. K-Nearest Neighbors (KNN)
- Tested for K values from 1 to 20 using 10-fold cross-validation.
- **Best Accuracy: 85.07% (K = 12)**

### 🌳 2. Decision Tree Classifier
- Evaluated depths from 1 to 10 using 10-fold cross-validation.
- **Best Accuracy: 78.77% (max_depth = 3)**

### 🌲 3. Random Forest Classifier
- Tried 10 to 100 estimators in steps of 10.
- **Best Accuracy: 83.82% (n_estimators = 90)**

---

## 📈 Results Comparison

| Model               | Best Accuracy |
|--------------------|---------------|
| K-Nearest Neighbors| 85.07%        |
| Decision Tree      | 78.77%        |
| Random Forest      | 83.82%        |

---

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/heart-disease-prediction.git
   cd heart-disease-prediction
