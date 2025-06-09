# 🧠 Customer Segmentation Dashboard using CORE + RFM (UrbanMart Project)

This project presents a customer segmentation solution built for UrbanMart, using **RFM scoring** and the strategic **CORE framework** (Convert, Optimize, Retain, Exit). Data processing was done in Python, and a single **interactive Tableau dashboard** was developed to visualize customer insights.

---

## 📁 Dataset Used

**File**: `UrbanMart_CORE_Segmentation_Enhanced.csv`  
**Records**: 2,000 transactions  
**Includes:**
- Customer demographics: `Gender`, `Age Group`, `Region`
- Purchase data: `TransactionDate`, `TransactionValue`, `ProductCategory`
- RFM metrics: `Recency`, `TransactionCount`, `Monetary`
- Scored fields: `R_Score`, `F_Score`, `M_Score`
- Tags: `CustomerType`, `Churn_Risk`, `Top_Spender`, `IsLoyalCustomer`
- Final segment: `CORE_Segment`

---

## 🛠 Tools & Technologies Used

| Tool               | Purpose                                      |
|--------------------|----------------------------------------------|
| **Python (Pandas)** | Data wrangling, feature engineering, RFM scoring |
| **Tableau**         | Interactive dashboard creation               |
| **GitHub**          | Project documentation                        |

---

## ✅ What Was Done

- Cleaned and transformed transaction data using Python
- Calculated **Recency, Frequency, and Monetary** values per customer
- Generated **RFM scores** (1 to 4 scale using quantiles)
- Applied logical tagging:
  - `CustomerType`: New or Repeat
  - `Top_Spender`: Upper quantile of spend
  - `IsLoyalCustomer`: Based on repeat frequency & recency
  - `Churn_Risk`: Inactive or high-risk customers
- Assigned each customer to a **CORE segment**:
  - **Convert**, **Optimize**, **Retain**, or **Exit**

---

## 📊 Tableau Dashboard Features

A single interactive dashboard includes:

### 🧮 KPI Tiles
- **Total Customers**
- **Average Spend per Customer**
- **Churn %**
- **% Loyal Customers**

### 📈 Visual Insights
- **CORE Segment Distribution** (Bar or Pie Chart)
- **CustomerType Breakdown by Age/Region**
- **Churn Risk Overview**
- **RFM Heatmap (Recency vs Frequency)**

### 🔍 Filters
- CORE Segment
- Customer Type
- Region
- Age Group
- Gender
- Churn Risk

All charts and KPIs are **interconnected** for real-time filtering and exploration.

---
