# 🚀 HR Promotion Prediction & Analytics Dashboard

---

## 🔷 Overview  
This project analyzes employee data to identify key factors influencing promotions and builds a machine learning model to predict high-potential employees.

The solution combines:
- Data Analysis (EDA)
- Machine Learning (Logistic Regression)
- Power BI Dashboard for decision-making

---

## 🔷 Problem Statement  
Organizations often struggle to:
- Identify employees ready for promotion  
- Maintain consistent promotion criteria  
- Avoid overlooking high-performing employees  

This project addresses these challenges using data-driven insights.

---

## 🔷 Dataset  
Employee demographic and performance data including:
- KPIs met  
- Previous year rating  
- Training score  
- Department, education, gender  

---

## 🔷 Approach  

### 1. Data Cleaning
- Removed empty columns and inconsistent headers  
- Handled missing values using median/mode  

---

### 2. Feature Engineering
Created **Fast Track** segment:
- KPI met = 1  
- Rating ≥ 4  
- Above-average training score  

---

### 3. Handling Class Imbalance
- Used `class_weight='balanced'` in Logistic Regression  
- Focused on improving recall instead of accuracy  

---

### 4. Model Building
- Logistic Regression with feature scaling  
- Evaluated using:
  - Precision  
  - Recall  
  - F1-score  

---

### 5. Threshold Tuning
- Adjusted classification threshold to optimize recall  

**Final Model Performance:**
- Recall: ~63%  
- Balanced precision  

---

### 6. Probability-Based Ranking
- Generated **promotion probability scores**  
- Ranked employees based on likelihood of promotion  

---

## 🔷 Key Insights  

- Employees meeting KPIs with high ratings and training scores are **~3x more likely** to be promoted  
- A large number of high-performing employees are **not promoted (promotion leakage)**  
- Previous year rating is one of the strongest predictors  

---

## 🔷 Dashboard Features (Power BI)

- KPI overview (Promotion rate, Fast Track rate)  
- Promotion drivers (KPI, rating, training score)  
- Fast Track analysis  
- Identification of **missed high-potential employees**  
- Top employees ranked by **promotion probability**  

---

## 🔷 Business Impact  

- Helps HR identify promotable employees proactively  
- Reduces bias in promotion decisions  
- Improves talent retention by highlighting overlooked employees  

---

## 🔷 Tech Stack  

- Python (Pandas, Scikit-learn)  
- Power BI  
- Excel  

---

## 🔷 Project Files  

- `promo.ipynb` → Model building  
- `hr_promotion_output` → Final dataset with probabilities  
- Power BI dashboard  

---

## 💡 Key Learning  

> Accuracy is not always the right metric — aligning model performance with business goals (recall in this case) is critical for real-world impact.

---

## 📌 Future Improvements  

- Use advanced models like Random Forest / XGBoost  
- Add more behavioral and performance features  
- Deploy as a web-based decision support tool  

---
