# Telco Customer Churn Analysis  

## 📌 Project Overview  
This project was completed as part of a **Code Institute** course, focusing on **data collection, processing, and machine learning** techniques to analyze **customer churn** for a telecommunications company.  

The workflow involves:  
- Fetching data from **Kaggle**  
- Cleaning and engineering features  
- Building **classification, regression, and clustering** models  
- Generating insights to help a client understand **churn patterns**  

---

## 📂 Project Structure  

### **1️⃣ Data Collection Notebook**  
**Objective:** Fetch and store raw data for analysis.  

- **Inputs:**  
  - `kaggle.json` (authentication token)  
- **Outputs:**  
  - `outputs/datasets/collection/TelcoCustomerChurn.csv`  

💡 *Note: In a real-world workplace, data usually comes from multiple sources like internal data warehouses, not Kaggle.*  

---

### **2️⃣ Churned Customer Study Notebook**  
**Objective:** Identify the key factors correlated with customer churn.  

- **Inputs:**  
  - `outputs/datasets/collection/TelcoCustomerChurn.csv`  
- **Outputs:**  
  - Analytical insights to be used in a **Streamlit App**  

---

### **3️⃣ Data Cleaning Notebook**  
**Objective:** Handle missing data and clean the dataset.  

- **Inputs:**  
  - `outputs/datasets/collection/TelcoCustomerChurn.csv`  
- **Outputs:**  
  - `outputs/datasets/cleaned/TrainSet.csv`  
  - `outputs/datasets/cleaned/TestSet.csv`  

🛠 **Key Cleaning Steps:**  
- Dropped unnecessary columns: `['customerID', 'TotalCharges']`  

---

### **4️⃣ Feature Engineering Notebook**  
**Objective:** Create new features for **classification, regression, and clustering models**.  

- **Inputs:**  
  - `outputs/datasets/cleaned/TrainSet.csv`  
  - `outputs/datasets/cleaned/TestSet.csv`  
- **Outputs:**  
  - List of engineered variables  

🛠 **Techniques Used:**  
- **Ordinal categorical encoding** for categorical variables  
- **Smart correlation selection** to identify key features  

---

### **5️⃣ Classification Model**  
**Objective:** Predict whether a customer will churn or not.  

- **Inputs:**  
  - `outputs/datasets/collection/TelcoCustomerChurn.csv`  
  - Cleaned and engineered features  
- **Outputs:**  
  - Model pipeline  
  - **Feature importance plot**  

---

### **6️⃣ Regression Model**  
**Objective:** Predict **tenure levels** for potential churners.  

- **Inputs:**  
  - Cleaned and engineered dataset  
- **Outputs:**  
  - ML pipeline for predicting tenure  
  - **Feature importance plot**  

---

### **7️⃣ Clustering Model**  
**Objective:** Group similar customers based on behavior.  

- **Inputs:**  
  - Cleaned and engineered dataset  
- **Outputs:**  
  - **Cluster profiles**  
  - **Silhouette analysis**  

---

## 🚀 Key Takeaways  
✅ **End-to-End ML Pipeline:** Data collection → Cleaning → Feature Engineering → Model Development  
✅ **Multiple ML Approaches:** Classification, Regression, Clustering  
✅ **Business Insights:** Helping businesses understand churn patterns  

---

## 🛠 Technologies Used  
- **Python**  
- **Pandas, NumPy, Scikit-learn**  
- **Matplotlib, Seaborn**  
- **Kaggle API**  
- **Streamlit (for visualization)**  



