# Employee Attrition Prediction – Executive Summary

---

## 🟦 Overview  
This project analyzes HR data to identify factors influencing employee attrition and builds a machine learning model to predict whether an employee is likely to leave the company.  
By leveraging historical employee data, the project aims to help organizations proactively address retention challenges.

---

## 🟥 Problem  
High employee turnover can lead to increased hiring costs, loss of organizational knowledge, and decreased productivity.  
Many companies struggle to identify at-risk employees early enough to intervene.  
The challenge was to develop a **data-driven solution** capable of predicting attrition while highlighting the most influential factors behind it.

---

## 🟨 Solution  
Using the **HR Analytics** dataset from Kaggle (~15,000 records, 10 features), the data was cleaned, analyzed, and visualized to uncover trends.  
Multiple classification models were built and evaluated (Logistic Regression, Decision Trees, Random Forest, and XGBoost), with the best-performing model selected based on **F1-score**, **precision**, **recall**, and **accuracy**.  
Key drivers of attrition were also identified to provide actionable insights for HR teams.

---

## 🟩 Details  

**Dataset Highlights:**  
- No missing values; data included satisfaction level, last evaluation score, number of projects, working hours, tenure, work accidents, promotions, department, and salary.  
- Target variable: `left` (1 = employee left, 0 = employee stayed).  
- Data cleaning involved outlier detection, encoding categorical variables, and scaling numerical features.

**Key Insights:**  
- Lower satisfaction levels and extremely high/low working hours were strong indicators of attrition.  
- Employees with very high evaluation scores but excessive working hours showed increased likelihood of leaving (possible burnout).  
- Lack of promotion over 5 years correlated with higher attrition.

### 📊 Model Performance – **Best Model: XGBoost Classifier**
| 🏆 Metric       | 📈 Score  |
|-----------------|----------|
| 🎯 **Precision** | **0.99** |
| 🔍 **Recall**    | **0.93** |
| 📏 **F1-Score**  | **0.96** |
| ✅ **Accuracy**  | **0.99** |

> **Highlight:** The XGBoost model delivers excellent precision and a high F1-score (0.96), indicating very strong predictive performance while maintaining reliable balance between precision and recall.


---

## 🟦 Next Steps  
- Collect additional data on employee engagement, training, and manager feedback.  
- Test model performance on real-time HR data for early attrition detection.  
- Integrate predictive insights into HR dashboards for proactive interventions.

---

## 📂 Repository Contents  
- `Employee_Attrition_Prediction.ipynb` – Full analysis, EDA, and model building.  
- Visualizations highlighting attrition patterns and key features.  
- Model evaluation reports and confusion matrix plots.
