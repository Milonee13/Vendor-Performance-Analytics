# Retail & Wholesale Inventory & Sales Analysis

## Business Problem
Effective inventory and sales management are critical for optimizing profitability in the retail and wholesale industry. Companies often face challenges such as:
- Inefficient pricing strategies leading to losses  
- Poor inventory turnover that increases holding costs  
- Over-reliance on specific vendors, creating supply chain risks  
- Ineffective promotional strategies for underperforming brands  

**This project aims to:**
- Identify underperforming brands for promotional or pricing adjustments  
- Determine top vendors contributing to sales and profitability  
- Analyze bulk purchasing impact on unit costs  
- Assess inventory turnover to reduce holding costs  
- Investigate profitability differences between high- and low-performing vendors  

---

## Data & Methodology

### Exploratory Data Analysis (EDA)
- **Summary Statistics**: Detected negative/zero gross profit, infinite margins, and unsold inventory.  
- **Outlier Detection**: Extreme variations in freight cost and purchase prices.  
- **Data Filtering**: Removed records with:  
  - Gross Profit ≤ 0  
  - Profit Margin ≤ 0  
  - Sales Quantity = 0  

### Correlation Analysis
- Weak relationship between purchase price and gross profit  
- Strong relationship (0.999) between purchase quantity and sales quantity  
- Negative relationship between sales price and profit margin (competitive pricing pressure)  
- Stock turnover weakly correlated with profit margin and gross profit  

### Hypothesis Testing
- **Null Hypothesis (H₀)**: No significant difference in profit margins between top- and low-performing vendors  
- **Result**: Rejected H₀ → significant profitability difference between vendor groups  

---

## Key Insights

### Promotional Adjustments
- 198 brands have low sales but high margins → strong candidates for targeted promotions  

### Vendor Dependence
- Top 10 vendors contribute **65.69% of purchases**, creating supply chain risk  

### Bulk Purchasing Benefits
- Large orders reduce unit costs by **72%** ($10.78 per unit vs higher costs in smaller orders)  

### Inventory Inefficiencies
- Unsold inventory capital = **$2.71M**, indicating slow-moving stock  

### Profitability Comparison
- Top Vendors → Avg. Margin = **31.17%**  
- Low Vendors → Avg. Margin = **41.55%** (higher margins but lower sales volumes)  

---

## Recommendations
- **Pricing Strategy**: Re-evaluate pricing of high-margin/low-sales brands to boost volume  
- **Vendor Diversification**: Reduce reliance on top 10 suppliers to mitigate risks  
- **Bulk Purchasing**: Leverage lower unit costs in large orders to maintain competitive pricing  
- **Inventory Optimization**:  
  - Reduce purchase quantities of slow-moving items  
  - Launch clearance sales or adopt optimized stocking policies  
- **Vendor-Specific Action**:  
  - Top Vendors → Focus on cost reduction and bundled promotions  
  - Low Vendors → Increase marketing, adjust pricing, and expand distribution  

---

## Tools & Technologies
- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy, Statsmodels)  
- SQL (purchase and sales data queries)  
- Jupyter Notebook (analysis and visualization)  

---

## Outcomes
By applying these recommendations, companies can:  
- Improve profitability through balanced pricing strategies  
- Mitigate supply chain risks with diversified vendors  
- Reduce holding costs via optimized inventory turnover  
- Enhance sales volumes while sustaining margins  
