# 📊 Vendor Insights Dashboard – Sales, Profit & Inventory Analysis
🔎 A data-driven project uncovering vendor performance, profitability trends, and inventory efficiency through exploratory data analysis and interactive dashboards.

## Data sources:
- Begin_inventory: [application_data.csv](https://drive.google.com/file/d/13pZjlqsOdcQ_Ttuayl-n9I1ZhQoXlx6E/view?usp=sharing)
- End_inventory:[application_data.csv](https://drive.google.com/file/d/1IsJTesCMROO7uBog8TQTJZ2DLd0LJu8I/view)
- Purchase_prices:[application_data.csv](https://drive.google.com/file/d/1fIRYlcrZzdiiL9_thATrq8nDShuQrNlU/view?usp=drive_open)
- Purchases:[application_data.csv]()
- Sales:[application_data.csv]()
- Vendor_invoice:[application_data.csv](https://drive.google.com/file/d/11OOriGMlVeOzj6Dou6ajOPe5RniLiQix/view)

## 📌 Dashboard Overview  
![PBI Dashboard - Vendor Insights](https://github.com/maheshyadavbattu/Vendor-Performance-Analytics-using-SQL-python-EDA-powerBI/blob/main/Dashboard%20View.png.png)  

## 🚀 Business Problem  

Effective inventory and sales management are crucial for profitability in the retail and wholesale industry. Companies must avoid losses due to inefficient pricing, poor inventory turnover, or vendor dependency.  

### Goals of this analysis:  
- Identify underperforming brands needing promotional or pricing adjustments  
- Determine top vendors contributing to sales & profit  
- Analyze the impact of bulk purchasing on unit costs  
- Assess inventory turnover to reduce holding costs  
- Investigate profitability variance between high & low-performing vendors  

---

## 🔍 Exploratory Data Analysis Insights  

### Negative & Zero Values  
- **Gross Profit:** Minimum = **-52,002.78**, indicating potential losses from heavy discounts or selling below cost.  
- **Profit Margin:** Minimum = **-∞**, caused by zero or negative revenue.  
- **Sales Quantity & Revenue:** Some products had **zero sales**, pointing to obsolete/slow-moving stock.  

### Outliers  
- **Purchase & Actual Prices:** Max = **7,499.99**, much higher than average (premium products).  
- **Freight Cost:** Ranges **0.09 → 257,032.07**, showing logistics inefficiencies.  
- **Stock Turnover:** Ranges **0 → 274.5**. Some products sell out fast, others remain unsold.  

### Data Filtering  
To ensure reliability, removed cases where:  
- Gross Profit ≤ 0  
- Profit Margin ≤ 0  
- Sales Quantity = 0  

---

## 📈 Correlation Insights  
- **Purchase Price vs. Sales & Profit:** Very weak correlation (-0.012, -0.016).  
- **Purchase Qty vs. Sales Qty:** Strong correlation (**0.999**) → efficient turnover.  
- **Profit Margin vs. Sales Price:** Negative correlation (-0.179), higher prices may reduce margins.  
- **Stock Turnover vs. Profitability:** Weak negative correlation.  

---

## ❓ Research Questions & Key Findings  

### 1️⃣ Brands for Promotional or Pricing Adjustments  
- 198 brands have **low sales but high margins** → need targeted marketing/promotions.  

### 2️⃣ Vendor Dependence  
- Top **10 vendors = 65.69%** of purchases.  
- High dependency → risk of supply chain disruptions.  

### 3️⃣ Bulk Purchasing Impact  
- Large quantity purchases lower unit cost by **72%** ($10.78 vs higher costs).  
- Encourages bigger orders → better sales & profitability.  

### 4️⃣ Low Inventory Turnover  
- **Unsold Inventory Capital = $2.71M**  
- Leads to storage costs, cash flow inefficiency.  

### 5️⃣ Profit Margin Comparison  
- **Top Vendors:** Mean = **31.17%**  
- **Low Vendors:** Mean = **41.55%**  
- Low vendors have higher margins but weaker sales volumes.  

### 6️⃣ Statistical Validation  
- **Hypothesis Testing Result:** Significant difference in profit margins between vendor groups.  
- **Implication:**  
  - High-margin vendors → need better marketing & distribution.  
  - Top-selling vendors → focus on cost efficiency.  

---

## ✅ Final Recommendations  

- Re-evaluate pricing for low-sales, high-margin brands.  
- Diversify vendor base to reduce risk.  
- Leverage bulk purchasing for cost savings.  
- Optimize slow-moving inventory (clearance sales, better purchasing strategy).  
- Enhance marketing & distribution for low-performing vendors.  
- Focus on sustainable profitability & operational efficiency.  
