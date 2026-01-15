# 📈 Insurance KPI & Claims Analytics

## 📝 Business Case
The goal of this project is to provide the executive team with a real-time view of insurance sales and claim processing efficiency. By tracking Monthly comparisons (CM vs PM), the company can identify shifts in risk and agent performance.

## 🛠️ Data Engineering & Modeling
* **Synthetic Data:** Generated via [Python Script](./generate_data.py) to simulate 2,500+ transactions.
* **Schema:** Star Schema with a central Date Table to support Time Intelligence.
* **Architecture:** 2 Fact Tables (Policies, Claims) linked to 4 Dimensions.

## 🧪 Advanced DAX Measures
I implemented several complex measures to track performance over time:
* **Time Intelligence:** `TOTALMTD`, `DATEADD`, and `SAMEPERIODLASTYEAR`.
* **Ratios:** Calculated Claim-to-Settlement ratios to identify high-loss product lines.
