# No-Show Predictor: Improving Patient Attendance with Machine Learning

An open-source machine learning system that predicts whether patients will attend their scheduled appointments, helping healthcare providers reduce missed appointments and improve service efficiency.

---

## 💡 Key Features
- Data cleaning and preprocessing (handling missing values, invalid ages, inconsistent labels)  
- Exploratory Data Analysis (EDA) with visualizations:
  - Missing values
  - Age distribution by Outcome and Diagnosis
  - Gender proportions by Diagnosis
  - GP Practice no-show rates
- Classification models: K-Nearest Neighbors (KNN) and Decision Tree  
- Evaluation with accuracy, confusion matrices, and classification reports  
- Feature importance and variance thresholding for model interpretability  
- Deployment-ready structure (Flask / Streamlit optional)  

---

## 🧠 Business Impact
Missed appointments increase costs, reduce patient care efficiency, and waste clinical resources.  
This project enables healthcare providers to **predict no-shows**, optimize scheduling, and improve patient outcomes.

> 💬 *Potential impact: reduce missed appointments by 20–30% and improve clinic efficiency.*

---

## 🧩 Dataset
**Dataset:** NHS patient appointment dataset  

Includes features such as:  
- Patient ID, Age, Gender  
- Diagnosis  
- GP Practice  
- Appointment Date  
- Appointment Outcome (Attended / Did Not Attend / variants)  

Target variable: **MissedAppointment** (binary: 1 = missed, 0 = attended)

---

## ⚙️ Technical Stack
| Category | Tools |
|-----------|-------|
| Data Analysis | Python, Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Deployment | Streamlit / Flask (optional) |

---

## 📈 Model Performance
| Model | Accuracy | F1-score (Missed) |
|-------|----------|------------------|
| K-Nearest Neighbors | 72% | 0.73 |
| Decision Tree | 71% | 0.72 |

The models achieve reasonable accuracy and can help identify patients at risk of missing appointments. Key predictive features include **Age, Diagnosis, GP Practice, and Gender**.

---

## 📊 Visual Results

### 🔹 Missing Values
Shows count of missing values by column before cleaning.

![Missing Values](images/missing_values.png)

---

### 🔹 Box Plot – Age by Outcome
Displays distribution of patient age by attendance outcome.

![Age by Outcome](images/age_boxplot.png)

---

### 🔹 KDE – Age by Outcome
Shows age distribution density by attendance outcome.

![Age Density](images/age_density.png)

---

### 🔹 No-Show Rate by GP Practice
Percentage of missed appointments by GP Practice.

![GP Practice No-Show Rate](images/no_show_gp.png)

---

### 🔹 Gender Proportion by Diagnosis
Pie charts visualizing male/female distribution per diagnosis.

![Gender by Diagnosis](images/gender_diagnosis.png)

---

### 🔹 Feature Retention
Retained vs. dropped features after variance thresholding.

![Feature Retention](images/feature_retention.png)

---

### 🔹 Confusion Matrix – KNN
Performance evaluation on test data.

![KNN Confusion Matrix](images/knn_confusion_matrix.png)

---

### 🔹 Confusion Matrix – Decision Tree
Performance evaluation on test data.

![Decision Tree Confusion Matrix](images/decision_tree_confusion_matrix.png)

---

### 🔹 No-Show Trend Over Time
7-day rolling average of missed appointments.

![Rolling Average](images/rolling_average.png)

---

## 🧮 Installation
```bash
git clone https://github.com/yourusername/no-show-predictor.git
cd no-show-predictor
pip install -r requirements.txt
