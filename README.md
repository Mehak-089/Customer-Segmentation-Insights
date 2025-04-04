# 🛍️ Customer Segmentation & RFM Insights Dashboard (E-Commerce Analytics)

[![Tableau Dashboard](https://img.shields.io/badge/View-Dashboard-blue)](https://public.tableau.com/views/CustomerSegmentationInsightsDashboard_17437831505140/Dashboard1)

## 📌 Overview

This project analyzes an e-commerce dataset using RFM (Recency, Frequency, Monetary) analysis and K-Means Clustering to segment customers based on purchasing behavior. The final output is an interactive Tableau dashboard that offers business insights for targeting customer groups effectively.

---

## 📊 Dashboard Link

🔗 **[Live Tableau Dashboard](https://public.tableau.com/views/CustomerSegmentationInsightsDashboard_17437831505140/Dashboard1)**  
> Explore cluster-wise customer behavior, purchasing patterns, and insights.

---

## 💼 Problem Statement

Businesses often struggle to understand customer behavior and personalize marketing efforts. This project solves this by segmenting customers into meaningful groups based on:
- How recently they purchased
- How frequently they purchase
- How much money they spend

---

## 🧰 Tools & Technologies

- **Python (Pandas, Sklearn, Matplotlib)**
- **K-Means Clustering (Unsupervised Learning)**
- **Tableau Public (Interactive Dashboard)**
- **Jupyter/VS Code (Data Preprocessing)**

---

## 📁 Dataset

- Source: Provided e-commerce sales data
- Contains ~500,000 transactions
- Features: `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## 🔍 Steps Performed

### 1. 📦 Data Cleaning & Feature Engineering
- Removed missing values and duplicates
- Filtered out canceled orders (negative quantities)
- Added `TotalPurchaseAmount = Quantity * UnitPrice`

### 2. 📈 RFM Analysis
- **Recency**: Days since last purchase  
- **Frequency**: Number of unique transactions  
- **Monetary**: Total spending by customer

### 3. 🤖 K-Means Clustering
- Normalized RFM values
- Used Elbow Method to find optimal number of clusters (K)
- Labeled customers into clusters (0–3)

### 4. 📊 Tableau Dashboard Design
- Imported `rfm_clustered_customers.csv` into Tableau
- Created extract and built visualizations:
  - Cluster-wise RFM averages
  - Customer count per cluster
  - Geographic and behavioral insights
- Added narrative insights using **Text Box**

---

## 📌 Key Insights

- **Cluster 2**: High-value, loyal customers. Frequent buyers with high monetary value.
- **Cluster 0**: Potentially valuable but need nurturing.
- **Cluster 1**: Dormant customers; can be reactivated via targeted campaigns.
- **Cluster 3**: Low activity; may be low-engagement customers.

---

## 🚀 Future Scope

- Add demographic segmentation (e.g., region, country)
- Use advanced models (e.g., DBSCAN, Hierarchical Clustering)
- Deploy dashboard in a business analytics environment (Power BI or Streamlit)

## 🧠 Author

**Mehak Memon**  
  
📧 mehakm5555@gmail.com | 

---



