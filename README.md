# Student Performance Prediction 🎓📊

This project predicts student academic performance categories (**Low, Medium, High**) using supervised machine learning. It leverages demographic, academic, and behavioral features to build a robust classification model using a **Random Forest Classifier**.

---

## 📌 Problem Statement
Educational institutions often struggle to identify students who may need academic support early. This project aims to predict student performance levels based on historical and behavioral data, enabling data-driven interventions.

---

## 📂 Dataset Overview
- **Total records:** 1000 (after cleaning: 960)
- **Features used:**
  - Gender
  - Previous Grade
  - Extracurricular Activities
  - Parental Support
  - Study Hours
  - Attendance (%)
  - Online Classes Taken
- **Target Variable:**
  - `GradeCategory` (Low, Medium, High)

Missing values were handled using:
- Median imputation for numerical features
- Mode imputation for categorical features

---

## 🛠️ Technologies & Libraries
- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**

---

## 🔍 Exploratory Data Analysis
- Correlation heatmap to understand feature relationships
- Grade category distribution visualization
- Detection and handling of missing values
- Removal of irrelevant identifiers (`StudentID`, `Name`)

---

## ⚙️ Feature Engineering
- Converted final numeric grades into categorical labels:
  - `Low` (0–55)
  - `Medium` (56–70)
  - `High` (71–100)
- One-hot encoding for categorical variables
- Stratified train-test split to preserve class distribution

---

## 🤖 Model Used
**Random Forest Classifier**
- `n_estimators`: 300  
- `max_depth`: 10  
- `min_samples_split`: 9  
- `random_state`: 42  

Chosen for its robustness, ability to handle mixed feature types, and resistance to overfitting.

---

## 📈 Model Performance
- **Accuracy:** 80.7%
- **Precision (Weighted):** 65.2%
- **Recall (Weighted):** 80.7%

⚠️ *Note:*  
A warning regarding undefined precision was observed due to one class receiving no predictions. This indicates **class imbalance and overlap** between performance categories.

---

## 🧾 Confusion Matrix
The confusion matrix provides insights into misclassification patterns among Low, Medium, and High performance categories, highlighting areas for potential model improvement.

---

## 🚀 Future Improvements
- Address class imbalance using SMOTE or class weighting
- Hyperparameter tuning using GridSearchCV
- Try alternative models (XGBoost, Gradient Boosting)
- Convert the project into a web-based prediction system
- Add explainability using SHAP or feature importance plots
---

## 👤 Author 

**Chakradhar Peddavenkatagari** 

Masters in Computer Science

The State University of New York at Buffalo 
