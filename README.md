# 📊 Vendor Performance analysis

## 🧩 Project Background 

Effective inventory and sales management are critical for optimizing profitability in the retail and wholesale industry. This project evaluates vendor performance and retail inventory dynamics to drive strategic insights for purchasing, pricing, and inventory optimization. The project objective aims to:

- Identify underperforming/overperforming vendors that require pricing or promotional adjustments  
- Determine top vendors contribution to sales and profits  
- Analyze the impact of bulk purchasing  
- Investigating inventory turnover inefficiencies  
- Statistically validate differences in vendor profitability  

This project uses vendor data, which includes 12 million records as a representative sample. The analysis demonstrates a systematic, data-driven methodology to uncover utilization management gaps and identify potential savings. 

---

## 🧠 Executive Summary


The business is efficient in purchasing, achieving up to **72% per-unit cost savings** through bulk orders and sourcing **65.69% of total purchases from its top 10 vendors**, indicating strong scale advantages.

**Key risks / constraints**
- It faces inventory inefficiencies, with approximately **$2.71 million in unsold stock** tying up working capital.
- It also faces **supplier concentration risk** due to heavy reliance on a small vendor base.

**Profitability opportunity**
- There is untapped profit potential in **40 low-volume, high-margin brands** and lower-volume vendors averaging **41.55% profit margins**, compared to **31.17% for high-volume vendors**, suggesting opportunities to improve overall profitability through better brand and vendor mix optimization.

**Main recommendations (executive-level)**
- **Diversify vendor partnerships** to reduce dependency on a limited number of suppliers and mitigate supply chain risks.
- **Optimize slow-moving inventory** by adjusting purchase quantities and using clearance initiatives to free up working capital.

---

## 🗂️ Data Structure

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/b0b959b0-9b23-4f6b-9983-0aa2552ff128" />


---

## 🔎 Insights Deep-Dive

Exploratory data analysis insights:

### Reliance on Top Vendors — Brief Summary

<img width="700" height="600" alt="image" src="https://github.com/user-attachments/assets/352df90f-2534-4f00-8b44-eee706bcb734" />


The Pareto analysis shows a **high concentration of purchasing among a small group of vendors**. The largest vendor alone accounts for approximately **16.3% of total purchases**, while the **top 10 vendors collectively contribute around 65–70%** of overall purchasing volume. This heavy reliance enables strong **bulk-purchasing cost efficiencies**, but it also introduces **supplier concentration risk**, increasing exposure to potential supply disruptions, pricing power imbalances, and dependency on a limited vendor base.


### ⚠️ Negative & Zero Values

**Gross Profit:**  
The minimum gross profit observed is –52,002.78, indicating potential losses driven by high costs or heavy discounting. This suggests that some products may have been sold at prices below their purchase cost.

**Profit Margin:**  
The profit margin reaches a minimum of –∞, which indicates cases where revenue is zero or lower than total costs, resulting in extremely negative margins.

**Total Sales Quantity & Sales Dollars:**  
Some products record zero sales quantity and zero sales revenue, indicating that these items were purchased but never sold. This points to slow-moving or obsolete inventory, contributing to overall inventory inefficiencies.

### 📌 Outliers Detected by High Standard Deviations

**Purchase & Actual Prices:**  
The maximum observed prices (5,681.81 for purchase price and 7,499.99 for actual price) are significantly higher than their respective means (24.39 and 35.64). This large gap indicates the presence of premium or high-value product offerings, which contribute to high variability in pricing.

**Freight Cost:**  
Freight costs exhibit extreme variation, ranging from 0.09 to 257,032.07, suggesting potential logistics inefficiencies, inconsistent shipment sizes, or irregular freight allocation across different products.

**Stock Turnover:**  
Stock turnover ranges from 0 to 274.5, indicating that while some products sell very rapidly, others remain unsold for extended periods. Turnover values greater than 1 imply that sales exceeded the quantity purchased during the period, likely due to existing inventory being used to fulfill orders.

---

## 📈 Research Questions & Key Findings

### 🧾 1. Brands for Promotional or Pricing Adjustments

<img width="975" height="625" alt="image" src="https://github.com/user-attachments/assets/1b06fe10-5557-4437-8bf3-1fa224f3ed4d" />


Around 40 brands exhibit lower sales but higher profit margins, indicating strong profitability potential. These brands could benefit from targeted marketing, selective promotions, or price optimization strategies to increase sales volume without compromising overall profitability.

### 📦 3. Impact of Bulk Purchasing on Cost Savings

<img width="666" height="220" alt="image" src="https://github.com/user-attachments/assets/8c3129be-e4d1-4659-b7e7-454a68d8b560" />


Vendors purchasing in large quantities achieve up to 72% lower unit costs ($10.78 per unit compared to significantly higher unit costs for smaller orders).  
Bulk pricing strategies incentivize larger order volumes, which increase total sales while preserving overall profitability.

### 🏷️ 4. Identifying Vendors with Low Inventory Turnover

<img width="625" height="531" alt="image" src="https://github.com/user-attachments/assets/054a3741-6dea-46c4-ab1b-375be53c0476" />



**Total Unsold Inventory Capital:** $2.71M  

Slow-moving inventory increases storage and holding costs, reduces cash-flow efficiency, and negatively impacts overall profitability.  
Identifying vendors with low inventory turnover allows the business to improve stock management, optimize purchasing decisions, and minimize financial strain caused by excess inventory.

### 📊 5. Profit Margin Comparison: High vs. Low-Performing Vendors

<img width="975" height="529" alt="image" src="https://github.com/user-attachments/assets/eb6c0caf-31b1-492f-a985-0afbdc465d9b" />


**Top Vendors’ Profit Margin (95% CI):** 30.74% – 31.61%  
**Mean:** 31.17%  

**Low-Performing Vendors’ Profit Margin (95% CI):** 40.48% – 42.62%  
**Mean:** 41.55%  

Low-performing vendors achieve higher profit margins but struggle with lower sales volumes, indicating potential pricing inefficiencies, limited market reach, or underutilized demand.

<img width="897" height="755" alt="image" src="https://github.com/user-attachments/assets/83073910-e81f-47c1-b177-667fd170c01c" />


### 🧪 6. Statistical Validation of Profit Margin Differences


**Hypothesis Testing:**  
- H₀ (Null Hypothesis): There is no significant difference in profit margins between top-performing and low-performing vendors.  
- H₁ (Alternative Hypothesis): A significant difference exists in profit margins between the two vendor groups.  

**Result:**  
The null hypothesis is rejected, confirming that the two vendor groups operate under distinctly different profitability models.

**Implication:**  
High-margin vendors may benefit from improved pricing or demand expansion strategies, while top-selling vendors should focus on cost efficiency and scale optimization to enhance margins.

---

## ✅ Recommendations

- Re-evaluate pricing strategies for low-sales, high-margin brands to increase sales volume without sacrificing profitability.
- Diversify vendor partnerships to reduce dependency on a limited number of suppliers and mitigate supply chain risks.
- Leverage bulk purchasing advantages to maintain competitive pricing while optimizing inventory levels.
- Optimize slow-moving inventory by adjusting purchase quantities, launching clearance initiatives, or revising storage and fulfillment strategies.
- Enhance marketing and distribution strategies for low-performing vendors to increase sales volumes without eroding profit margins.
- By implementing these recommendations, the company can achieve sustainable profitability, reduce operational risk, and improve overall operational efficiency.
