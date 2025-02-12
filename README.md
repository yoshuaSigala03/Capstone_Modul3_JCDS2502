# Capstone_Modul3_JCDS2502
# 📊 Bank Marketing Campaign Classification  

## 📌 Project Overview  
This project focuses on **predicting customer deposits** in a bank marketing campaign using **classification models**. The goal is to optimize marketing efforts by targeting potential deposit customers efficiently, **maximizing revenue while reducing unnecessary costs**.  

## 🔹 Key Steps in the Analysis  
### **1️⃣ Data Preprocessing & Feature Engineering**  
- **Handled missing values** (median for numerical, most frequent for categorical).  
- **Scaled numerical features** using **RobustScaler** to handle outliers.  
- **Encoded categorical features** via **One-Hot Encoding & Ordinal Encoding** for better model compatibility.  
- **Created new features:**  
  - **Age groups** for customer segmentation.  
  - **Balance categories** to identify high-value clients.  
  - **Previous contact status** as a key predictor.  

### **2️⃣ Exploratory Data Analysis (EDA)**  
- Identified a **slight class imbalance (47% deposits, 53% no deposits)**.  
- Found strong correlations between deposits and factors like **age, balance, and previous contact success**.  
- Addressed **outliers in balance and campaign features** to prevent bias in modeling.  

### **3️⃣ Model Training & Evaluation**  
- Compared **7 classification models** using **5-fold cross-validation**:  
  - **Gradient Boosting initially performed best (F1-score: 67.9%)**  
  - **Random Forest performed best after hyperparameter tuning (F1-score: 68.42%)**  
- **Applied SMOTE** to handle class imbalance, improving recall but slightly increasing false positives.  
- **Final threshold tuning (0.36) provided the best financial results.**  

### **4️⃣ Cost-Benefit Analysis**  
- **Evaluated financial impact** of model decisions using real-world cost-benefit calculations.  
- **Final model achieved the highest net benefit ($673,332),** a **145% increase** from the baseline.  

---

## 🚀 Final Recommendation  
- **Deploy the optimized Random Forest model (Threshold 0.36)** to maximize **deposit conversions & revenue**.  
- **Target high-value customer segments** (ages 41-60, higher balances, previous successful contacts).  
- **Optimize marketing strategies** to reduce false positives & unnecessary costs.  
- **Continuously retrain and monitor the model** to adapt to changing customer behavior.  

---

## 📌 Technologies Used  
- **Python (Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn)**  
- **Machine Learning (Random Forest, Gradient Boosting, XGBoost, AdaBoost, Logistic Regression, KNN, Decision Tree)**  
- **Imbalanced Learning (SMOTE)**  
- **Hyperparameter Tuning (RandomizedSearchCV, GridSearchCV)**  

---

