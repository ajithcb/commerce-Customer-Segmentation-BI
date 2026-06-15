# 📊 E-Commerce Customer Segmentation & Performance Analytics

## 📝 Project Overview
This project transforms raw transactional data from an online retail business into actionable business insights. Using **Python** for data engineering and **Power BI** for visual storytelling, I built an RFM (Recency, Frequency, Monetary) segmentation model to categorize customers and help marketing teams target them efficiently.

---

## 🛠️ Tech Stack & Tools Used
* **Data Engineering & Cleaning**: Python (Pandas, Datetime) via Google Colab
* **Segmentation Framework**: RFM Modeling (Recency, Frequency, Monetary value)
* **Data Visualization**: Power BI Desktop
* **Version Control**: Git & GitHub

---

## ⚙️ Technical Blueprint & Logic
1. **Data Cleaning**: Managed structural missing values by systematically dropping records lacking valid customer identifications. Filtered out canceled transactions and zero-value unit pricing models.
2. **Feature Engineering**: Formulated a runtime script grouping records by individual customer IDs to calculate:
   * **Recency**: Elapsed days since the customer’s latest transaction baseline.
   * **Frequency**: Total discrete order occurrences.
   * **Monetary**: Total lifetime spending (`Quantity` × `UnitPrice`).
3. **Algorithmic Scoring**: Distributed customer scores on a quantile rank matrix to dynamically generate targeted marketing streams.

---

## 🔮 Core Insights Formulated
* **VIP Champions**: High-frequency, high-spending customers who drive the majority of the business's total revenue.
* **At-Risk Cohorts**: Customers who previously purchased frequently but have not interacted recently, representing an immediate marketing re-engagement opportunity.
* **New / Recent Customers**: High recency but low frequency buyers who require onboarding campaigns to turn them into repeat purchasers.

---

## 🗄️ Repository Contents
* `Ecommerce_Customer_Segmentation.pbix`: Complete interactive Power BI dashboard tracking revenue, segments, and distinct customer metrics.
* `Ecommerce_Customer_Segments.csv`: Processed output dataset containing final customer RFM metrics and cohort assignments.
* `*.ipynb`: Python source script containing data cleaning, missing value handling, and algorithmic RFM calculations.
