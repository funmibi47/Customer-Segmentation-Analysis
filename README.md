# 📊 Customer Segmentation Analysis  
*A Data Analytics Project using RFM Analysis & K-Means Clustering*

---

## 📌 Project Overview  
This project performs **customer segmentation** for an e-commerce business using purchase behavior.  
The goal is to group customers based on their:

- Recency (How recently they purchased)
- Frequency (How often they purchased)
- Monetary (How much they spent)

Segmentation helps the business improve marketing strategies, customer retention, and product recommendations.

---

## 📁 Dataset  
The dataset contains typical e-commerce transaction details:

| Column | Description |
|--------|-------------|
| **InvoiceNo** | Unique invoice number (C-prefixed values = cancellations) |
| **StockCode** | Unique product code |
| **Description** | Product name |
| **Quantity** | Units purchased (negative = returns) |
| **InvoiceDate** | Purchase timestamp |
| **UnitPrice** | Price per item |
| **CustomerID** | Unique customer identifier |
| **Country** | Customer location |

Dataset source: **Kaggle**

---

## 🛠️ Tools & Technologies  
- Python  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- Jupyter Notebook  
- GitHub  

---

## 🔍 Project Steps  

### 1️⃣ Data Cleaning & Preparation
- Removed negative quantities (returns)  
- Removed cancelled invoices (`InvoiceNo` starting with “C”)  
- Dropped rows with missing `CustomerID`  
- Converted `InvoiceDate` to datetime  
- Created a new column:

🎯 Key Insights

Cluster 0: High spenders, frequent buyers

Cluster 1: Low-value customers

Cluster 2: Recent but low-frequency customers

Cluster 3: At-risk customers (long recency)

These insights help personalize campaigns and increase revenue.
