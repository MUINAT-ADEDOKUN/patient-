# No-Show Predictor: Improving Patient Attendance with Machine Learning

An open-source machine learning system that predicts whether patients will attend their scheduled healthcare appointments. This project helps healthcare providers reduce missed appointments and improve operational efficiency using data-driven insights.

This work demonstrates the practical application of **machine learning, data analysis, and predictive modeling** to a real-world healthcare problem.

---

## 💡 Key Features

### 🔹 Data Preparation
- Comprehensive data cleaning and preprocessing  
- Handling missing values  
- Fixing invalid ages  
- Standardizing inconsistent appointment outcome labels  

### 🔹 Exploratory Data Analysis (EDA)
- Missing data analysis  
- Age distribution by outcome and diagnosis  
- Gender proportions by diagnosis  
- GP practice–level no-show rates  
- Time-based no-show trends  

### 🔹 Machine Learning
- Feature engineering and variance thresholding  
- Classification models:
  - K-Nearest Neighbors (KNN)  
  - Decision Tree Classifier  

### 🔹 Model Evaluation
- Accuracy  
- Precision, Recall, and F1-score  
- Confusion matrices  

### 🔹 Reproducibility & Deployment
- Reproducible workflow with all charts saved programmatically  
- Deployment-ready structure (Streamlit / Flask optional)  

---

## 🧠 Business Impact

Missed healthcare appointments lead to:
- Increased operational costs  
- Inefficient use of clinical resources  
- Reduced quality of patient care  

This project enables healthcare providers to:
- Predict patients at risk of missing appointments  
- Implement targeted reminders or scheduling interventions  
- Improve clinic efficiency and patient outcomes  

> **Potential Impact:**  
> Reduce missed appointments by **20–30%** through predictive analytics and early intervention.

---

## 🧩 Dataset

**Dataset:** NHS patient appointment dataset  

### Included Features
- Patient ID  
- Age  
- Gender  
- Diagnosis  
- GP Practice  
- Appointment Date  
- Appointment Outcome  

### 🎯 Target Variable
**MissedAppointment**
- `1` = Missed appointment  
- `0` = Attended appointment  

---

## ⚙️ Technical Stack

| Category | Tools |
|--------|------|
| Programming | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Deployment (Optional) | Streamlit, Flask |

---

## 👩‍💻 My Role and Contributions
- Designed and implemented the end-to-end machine learning pipeline  
- Cleaned and standardized raw NHS appointment data  
- Conducted exploratory data analysis and feature engineering  
- Built and evaluated KNN and Decision Tree models  
- Applied variance thresholding for feature selection  
- Interpreted model outputs into actionable healthcare insights  
- Saved and documented all visual outputs for reproducibility  

---

## 🚀 Innovation and Technical Value
- Applies machine learning to real-world public healthcare operations  
- Transforms raw appointment data into predictive decision-support tools  
- Demonstrates scalable analytics applicable to healthcare systems  
- Bridges data science, machine learning, and operational impact  

---

## 📈 Model Performance

| Model | Accuracy | F1-score (Missed) |
|------|----------|------------------|
| K-Nearest Neighbors (KNN) | 74% | 0.75 |
| Decision Tree | 71% | 0.72 |

**Key predictive features:** Age, Diagnosis, GP Practice, Gender

---

## 📊 Visual Results

### 🔹 Missing Values
Shows count of missing values by column before cleaning.

![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/34b7222b5c37239af7187e98485f767039458e3c/Missing_Data.png)

---

### 🔹 Box Plot – Age by Outcome
Displays distribution of patient age by attendance outcome.

![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/34b7222b5c37239af7187e98485f767039458e3c/Box_Plot_Age_by_Outcome.png)

---

### 🔹 KDE – Age by Outcome
Shows age distribution density by attendance outcome.

![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/34b7222b5c37239af7187e98485f767039458e3c/(KDE)_by_Outcome.png)

---


### 🔹 Gender Proportion by Diagnosis
Pie charts visualizing male/female distribution per diagnosis.
![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/e194ce857465058250417bc6437d4623401b1f75/Gender_Proportion_Asthma.png)
![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/e194ce857465058250417bc6437d4623401b1f75/Gender_Proportion_Diabetes.png)
![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/e194ce857465058250417bc6437d4623401b1f75/Gender_Proportion_Hypertension.png)
![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/e194ce857465058250417bc6437d4623401b1f75/Gender_Proportion_Unknown.png)

---

### 🔹 Feature Retention
Retained vs. dropped features after variance thresholding.

![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/34b7222b5c37239af7187e98485f767039458e3c/Retained_and_Dropped_Features_after_Variance_Thresholding.png)
---

### 🔹 Confusion Matrix – KNN
Performance evaluation on test data.

![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/34b7222b5c37239af7187e98485f767039458e3c/KNN_confusion_matrix.png)

---

### 🔹 Confusion Matrix – Decision Tree
Performance evaluation on test data.

![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/34b7222b5c37239af7187e98485f767039458e3c/Decision%20Tree%20Model%20Performance.png)
---

### 🔹 No-Show Trend Over Time
7-day rolling average of missed appointments.

![image alt](https://github.com/MUINAT-ADEDOKUN/patient-/blob/34b7222b5c37239af7187e98485f767039458e3c/7-Day_Rolling_Average_Missed_Appointments.png)
---

## 🧮 Installation
```bash
git clone https://github.com/yourusername/no-show-predictor.git
cd no-show-predictor
pip install -r requirements.txt
