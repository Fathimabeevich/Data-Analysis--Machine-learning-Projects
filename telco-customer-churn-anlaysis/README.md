# 📊 Customer Churn Segmentation Using K-Means Clustering
This project analyzes the **Telco Customer Churn dataset** and applies **K-Means clustering** to segment customers into meaningful groups based on their billing behavior, service usage, and churn history.  
The goal is to help telecom providers understand customer patterns and create better retention strategies.

## 🚀 Project Overview

This project includes:

- Data Cleaning & Preprocessing  
- Exploratory Data Analysis (EDA)  
- Encoding Categorical Features  
- Feature Scaling  
- K-Means Clustering (K = 3)  
- Customer Segment Analysis  
- Business Insights and Recommendations  

---

## 🛠️ Tech Stack

- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Scikit-learn**
- **Jupyter Notebook**

---

## 📥 Dataset

The project uses the **Telco Customer Churn** dataset, which includes:

- Customer demographic details  
- Account / contract information  
- Billing and charges  
- Service subscriptions  
- Churn history (Yes/No)

---

## 🔧 Data Preprocessing

### ✔ Handled missing values  
### ✔ Cleaned service columns:
Converted values such as `"No internet service"` → `"No"`  
Converted `"Yes"` / `"No"` to **1 / 0**

### ✔ Label Encoding for binary columns:
- gender  
- Partner  
- Dependents  
- PhoneService  
- OnlineSecurity  
- TechSupport  
- StreamingTV  
- StreamingMovies  

### ✔ One-Hot Encoding for multi-category columns:
- InternetService  
- Contract  
- PaymentMethod  

### ✔ Converted "TotalCharges" to numeric and filled missing values  

### ✔ Dropped unnecessary features like `customerID`

---

## 📊 Exploratory Data Analysis

- Churn distribution  
- Tenure distribution  
- Charges distribution  
- Correlation heatmap  
- Service usage patterns  

---

## 🤖 K-Means Clustering

### ✔ Selected features:
- Tenure  
- MonthlyCharges  
- TotalCharges  
- Encoded service usage  
- Contract type  
- Internet service type  
- Payment method  

### ✔ Scaled features using StandardScaler  
### ✔ Used Elbow Method → **Optimal K = 3**

---

## 🧩 Customer Segments Identified

### **🔵 Segment 0 — Mid-Value Moderate Risk**
- Medium monthly charges  
- Moderate service usage  
- Average tenure  
- Churn rate: **25%**  
- Target: engagement programs  

---

### **🟢 Segment 1 — Low-Value Loyal Customers**
- Low monthly charges  
- Basic plans  
- Very few services  
- Lowest churn: **7%**  
- Target: upsell opportunities  

---

### **🔴 Segment 2 — High-Value Premium, High Churn**
- Highest monthly charges  
- Use many premium services  
- Highest churn: **33%**  
- Target: retention strategy  

---

## 💡 Business Recommendations

- Focus retention offers on **Segment 2** (high-value, high-churn)  
- Upsell additional services to **Segment 1** (loyal but low revenue)  
- Improve long-term engagement for **Segment 0**  
