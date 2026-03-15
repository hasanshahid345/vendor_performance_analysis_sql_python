# 📊 Vendor Performance Analysis

## 🧩 Project Background

Effective inventory and sales management are critical for optimizing profitability in the retail and wholesale industry. This project evaluates vendor performance and implements an end-to-end data analysis and machine learning workflow designed to support finance and procurement teams by:

- Predicting expected freight costs for vendor invoices  
- Identifying underperforming and overperforming vendors that require pricing or promotional adjustments  
- Statistically validating differences in vendor profitability  

The project uses vendor data containing **12 million records** as a representative sample. The analysis demonstrates a systematic, data-driven methodology to uncover utilization management gaps and identify potential savings.

---

# 🧠 Executive Summary

The business demonstrates strong purchasing efficiency, achieving up to **72% per-unit cost savings** through bulk orders and sourcing **65.69% of total purchases from its top 10 vendors**, indicating strong scale advantages.

## Key Risks & Constraints

- Approximately **$2.71 million in unsold inventory** is tying up working capital.
- There is **supplier concentration risk**, as the business relies heavily on a small group of vendors.

## Profitability Opportunity

There is untapped profit potential in **40 low-volume, high-margin brands** and lower-volume vendors averaging **41.55% profit margins**, compared to **31.17% for high-volume vendors**. This suggests opportunities to improve overall profitability through better brand and vendor mix optimization.

## Executive Recommendations

- **Diversify vendor partnerships** to reduce dependency on a limited number of suppliers and mitigate supply chain risks.
- **Optimize slow-moving inventory** by adjusting purchase quantities and implementing clearance initiatives to free up working capital.

---

# 🗂️ Data Structure

![Data Structure](image-4.png)

---

# 🔎 Exploratory Data Analysis Insights

## ⚠️ Negative & Zero Values

### Gross Profit
The minimum gross profit observed is **–52,002.78**, indicating potential losses driven by high costs or heavy discounting. Some products may have been sold below their purchase cost.

### Profit Margin
Profit margins reach **–∞**, indicating cases where revenue is zero or lower than total costs.

### Sales Quantity & Sales Dollars
Some products record **zero sales quantity and zero revenue**, indicating purchased items that were never sold. This contributes to slow-moving or obsolete inventory.

---

## 📌 Outliers Detected by High Standard Deviations

### Purchase & Actual Prices
Maximum prices (**5,681.81 purchase price** and **7,499.99 actual price**) are far above their respective means (**24.39** and **35.64**), indicating premium product segments.

### Freight Cost
Freight costs vary dramatically (**0.09 – 257,032.07**), suggesting possible logistics inefficiencies or irregular shipment allocations.

### Stock Turnover
Stock turnover ranges from **0 to 274.5**, indicating that while some products sell rapidly, others remain unsold for long periods.

---

# 📈 Research Questions & Key Findings

## 🧾 1. Brands for Promotional or Pricing Adjustments

![Brand Analysis](image-3.png)

Approximately **40 brands** exhibit lower sales but higher profit margins. These brands present opportunities for targeted marketing or selective promotions to increase sales while maintaining strong profitability.

---

## 📦 2. Impact of Bulk Purchasing on Cost Savings

![Bulk Purchasing](image-2.png)

Vendors purchasing in large quantities achieve up to **72% lower unit costs** ($10.78 per unit compared to significantly higher costs for smaller orders).

Bulk pricing strategies incentivize larger order volumes while preserving profitability.

---

## 🏷️ 3. Identifying Vendors with Low Inventory Turnover

![Inventory Turnover](image-1.png)

**Total Unsold Inventory Capital:** $2.71M

Slow-moving inventory increases holding costs, reduces cash-flow efficiency, and negatively impacts profitability.

Identifying vendors with low turnover helps improve purchasing decisions and inventory management.

---

## 📊 4. Profit Margin Comparison: High vs Low Performing Vendors

![Profit Margin Comparison](image.png)

| Vendor Type | Profit Margin (95% CI) | Mean |
|--------------|-----------------------|------|
| Top Vendors | 30.74% – 31.61% | 31.17% |
| Low-Performing Vendors | 40.48% – 42.62% | 41.55% |

Low-performing vendors achieve higher margins but struggle with lower sales volumes, suggesting underutilized demand or pricing inefficiencies.

---

## 🧪 5. Statistical Validation of Profit Margin Differences

**Hypothesis Testing**

- **H₀:** No significant difference in profit margins between vendor groups  
- **H₁:** Significant difference exists between vendor groups  

**Result:**  
The null hypothesis is rejected.

**Implication:**  
Different vendor groups operate under distinct profitability models.

High-margin vendors may benefit from demand expansion strategies, while high-volume vendors should focus on cost efficiency and scale optimization.

---

# 🎯 Machine Learning Objective

## Freight Cost Prediction (Regression)

**Goal:**  
Predict the expected freight cost for vendor invoices using invoice quantity, invoice value, and historical transaction patterns.

### Business Importance

- Freight is a major component of landed cost
- Accurate freight prediction improves budgeting
- Enables better procurement planning and vendor negotiations

---

# 🤖 Models Used

## Regression Models

- Linear Regression *(baseline)*
- Decision Tree Regressor
- Random Forest Regressor *(final model)*

## Classification Models (Invoice Flagging)

- Logistic Regression *(baseline)*
- Decision Tree Classifier
- Random Forest Classifier *(final model tuned with GridSearchCV)*

Hyperparameter tuning uses **GridSearchCV with F1-score** to address class imbalance.

---

# 📊 Evaluation Metrics

## Freight Prediction

- **MAE** – Mean Absolute Error  
- **RMSE** – Root Mean Squared Error  
- **R² Score**

---

# ⚙️ How to Run This Project

## 1. Clone Repository

```bash
git clone https://github.com/hasanshahid345/vendor_performance_analysis_sql_python.git
cd vendor_performance_analysis_sql_python
