# Fraud Detection for Business Context

## 📌 Overview
This project focuses on detecting fraudulent transactions in a business context using machine learning techniques.  
The dataset contains over **6 million transaction records** with attributes such as transaction type, amount, origin and destination balances.  
The goal is to build and evaluate models that can accurately identify fraudulent activities.

---

## 📂 Dataset
- **Source**: `Fraud.csv`
- **Size**: 6,362,620 entries, 11 columns
- **Key Features**:
  - `type`: Transaction type (CASH-IN, CASH-OUT, PAYMENT, TRANSFER, DEBIT)
  - `amount`: Transaction amount
  - `oldbalanceOrg`, `newbalanceOrg`: Origin account balances
  - `oldbalanceDest`, `newbalanceDest`: Destination account balances
  - `isFraud`: Label indicating actual fraud
  - `isFlaggedFraud`: Flagged suspicious transactions

---

## ⚙️ Tech Stack
- **Language**: Python  
- **Libraries**:
  - `pandas`, `numpy` → Data handling  
  - `matplotlib`, `seaborn` → Visualization  
  - `scikit-learn` → ML models (Logistic Regression, Random Forest), preprocessing, metrics  

---

## 🚀 Workflow
1. **Data Exploration**
   - Checked missing values, duplicates, and data distribution.
   - Visualized fraud vs. non-fraud transactions.
   - Analyzed fraud rates across transaction types.

2. **Preprocessing**
   - Encoded categorical features (`LabelEncoder`).
   - Scaled numerical values (`StandardScaler`).
   - Addressed class imbalance using **resampling**.

3. **Modeling**
   - Implemented **Random Forest Classifier** and **Logistic Regression**.
   - Split dataset into training and testing sets.

4. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC.
   - Confusion Matrix & ROC Curve plots.

---

## 📊 Results
- Fraudulent transactions are extremely **imbalanced** compared to legitimate ones.
- **Random Forest** performed better than Logistic Regression in terms of recall and AUC, making it more reliable for fraud detection.
- Visualization highlighted transaction patterns that can help in real-world monitoring.

---

## ▶️ How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Fraud-Detection-Business.git
   cd Fraud-Detection-Business
