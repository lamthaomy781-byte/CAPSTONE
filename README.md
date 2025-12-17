# 📊 CAPSTONE PROJECT  
## Customer Value Analysis & VIP Prediction using RFM and KNN

---

## 📌 Project Overview

This Capstone project focuses on **Customer Value Analysis** using the  
**RFM model (Recency – Frequency – Monetary)** combined with  
**Machine Learning (K-Nearest Neighbors – KNN)** and **Power BI visualization**.

The project is built on the **Online Retail Dataset** with the purpose of:
- Analyzing customer purchasing behavior
- Segmenting customers based on value
- Identifying and predicting **VIP customers**
- Detecting extreme customer imbalance
- Providing **data-driven business insights and recommendations**

---

## 🎯 Business Objectives

- Calculate and analyze **RFM metrics**
- Segment customers into **DELUX – STANDARD – VIP**
- Identify **Extreme Customer Imbalance**
- Predict potential VIP customers using **KNN**
- Visualize results through **Power BI dashboards**
- Support strategic business decision-making

---

## 🔍 Methodology

### Data Cleaning and Preparation
- Remove cancelled transactions
- Handle missing values
- Create **Revenue = Quantity × Price**
- Convert and standardize date formats

### RFM Calculation
For each customer:
- **Recency (R):** Days since last purchase
- **Frequency (F):** Number of transactions
- **Monetary (M):** Total spending value

### RFM Scaling and Scoring
- Apply **MinMaxScaler**
- Adjust Recency so that lower recency corresponds to higher score
- Compute a weighted RFM score using the formula:

RFM_SCORE = 0.3 × R_adj + 0.5 × F_scaled + 0.2 × M_scaled


### Customer Segmentation
Based on the RFM score, customers are classified into:
- **DELUX:** Low-value, high-risk customers
- **STANDARD:** Medium-value customers with growth potential
- **VIP:** High-value and most critical customers

### Machine Learning – KNN
- **Input features:** R_scaled, F_scaled, M_scaled
- **Target variable:** VIP_Label
- **Model:** K-Nearest Neighbors (KNN)
- **Objective:** Predict potential VIP customers

---

## 📊 Key Insights from the Analysis

### Extreme Customer Imbalance
- **DELUX:** Approximately **99.5%** of total customers
- **VIP:** Approximately **0.03%** (only 2 customers)

This indicates that business revenue is **highly concentrated** in a very small group of customers.

### Dormancy Risk
- Average Recency of DELUX customers is approximately **202 days**
- Most customers have not made a purchase for more than **6 months**

This reflects a serious customer retention issue and highlights the need for win-back strategies.

### VIP Segment
- Average purchase frequency: **~367 transactions**
- Average monetary value: **~176,000**
- Represents the **core revenue source** of the business

VIP customers require personalized service and maximum retention effort.

### STANDARD Segment
- Good recency and high purchase frequency
- Strong potential to be upgraded to VIP

This segment is the primary target for **upsell and cross-sell strategies**.

---

## 📈 Power BI Dashboard

The Power BI dashboard includes:
- KPI Cards (Total Customers, VIP Count, Average RFM Score)
- Customer Distribution by RFM Segment
- VIP vs Regular Customer Comparison
- RFM Score Distribution
- Customer Positioning (Recency vs Frequency)
- Business Insights and Recommendations section

---

## 🛠️ Tools and Technologies

- **Python:** pandas, numpy, matplotlib, seaborn, scikit-learn
- **Jupyter Notebook**
- **Power BI**
- **Git & GitHub**

---

## 📌 Conclusion and Recommendations

- Prioritize retention of **VIP customers**
- Develop conversion strategies from **STANDARD to VIP**
- Reduce marketing costs for inactive DELUX customers
- Use RFM analysis as a foundation for data-driven business decisions



