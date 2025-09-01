# IBM HR Analytics Employee Attrition Prediction  

![Python](https://img.shields.io/badge/Python-3.9-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-ScikitLearn-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-optimized-brightgreen)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
Employee attrition is a critical concern for organizations. This project leverages **Machine Learning techniques** to analyze and predict employee attrition, enabling HR teams to proactively retain talent and reduce turnover costs.

---

## 🎯 **Objective**
- Predict which employees are most likely to leave the organization.
- Provide actionable insights to assist HR teams in making data-driven retention decisions.

---

## 🛠 **Tech Stack**
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost  
- **Techniques:** Feature Engineering, Cross-Validation, Hyperparameter Tuning, Class Balancing  

---

## 📂 **Project Workflow**
1. **Data Cleaning & Preprocessing**
   - Removed missing and duplicate records.
   - Encoded categorical variables using **Label Encoding**.
   - Standardized numerical features with **StandardScaler**.
   
2. **Exploratory Data Analysis (EDA)**
   - Univariate & Bivariate Analysis for feature insights.
   - Correlation heatmaps to detect multicollinearity.
   - Boxplots to identify outliers.
   
3. **Feature Selection**
   - Identified significant features using **Feature Importance** from Random Forest and XGBoost.
   - Reduced dimensionality for improved model efficiency.
   
4. **Model Building & Evaluation**
   - Algorithms used:
     - Logistic Regression  
     - Random Forest  
     - SVM  
     - **XGBoost**  
   - Evaluated models with **5-Fold Cross Validation** using metrics like Accuracy, Precision, Recall, F1-Score, and ROC-AUC.
   
5. **Class Imbalance Handling**
   - Applied `scale_pos_weight` in XGBoost and class weights for Random Forest.
   - Boosted recall to ensure more accurate prediction of attrition cases.

6. **Hyperparameter Tuning**
   - Tuned XGBoost with **GridSearchCV** for optimized performance.

---

## 📊 **Model Performance**
| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|--------|----------|-----------|--------|----------|----------|
| Logistic Regression | ~0.85 | Medium | Low | Low | ~0.77 |
| Random Forest | ~0.85 | High | ~0.20 | ~0.31 | ~0.78 |
| SVM | ~0.84 | Medium | Low | Low | ~0.76 |
| **XGBoost** | ~0.85 | Medium | **~0.40** | **~0.45** | ~0.77 |

---

## 🔑 **Key Insights**
- Employees working **OverTime** are more prone to attrition, indicating workload stress.
- **Lower MonthlyIncome** correlates with higher attrition risk.
- Employees with **short or very long tenure** have higher attrition chances.
- **JobSatisfaction** plays a significant role in retention.

---

## 🚀 **How to Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/IBM-HR-Analytics-Attrition.git
