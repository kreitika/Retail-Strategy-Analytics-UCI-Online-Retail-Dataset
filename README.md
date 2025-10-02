# 🛍️ Retail Strategy Analytics – Driving Growth Through Customer & Product Insights

This project applies business analytics on the **UCI Online Retail Dataset** (~500k UK retail transactions) to generate actionable customer and product insights.  
The analysis was performed in **Python (Google Colab)** and visualized with **Tableau**.

---

## 📊 Dashboard

👉 [**View the Interactive Tableau Dashboard**](https://public.tableau.com/authoring/RetailStrategyAnalyticsUCIOnlineRetailDataset/RetailStrategyAnalyticsUCIOnlineRetailDataset#2) 


---

## 📂 Dataset
- Source: [UCI Machine Learning Repository – Online Retail](https://archive.ics.uci.edu/ml/datasets/online+retail)  
- Transactions from a UK-based online store (Dec 2010 – Dec 2011).  
- Columns: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country.

---

## 🛠️ Tools & Libraries
- **Python:** Pandas, NumPy, Matplotlib, scikit-learn, lifetimes, mlxtend  
- **SQL:** DuckDB for exploratory queries  
- **Visualization:** Tableau Public  
- **Environment:** Google Colab, Mac (local for Tableau)  

---

## 🔎 Approach

1. **Data Cleaning**
   - Removed cancelled invoices and negative quantities.
   - Calculated per-order revenue.
   - Filtered for valid CustomerIDs.

2. **Customer Segmentation (RFM Analysis)**
   - Recency, Frequency, Monetary (RFM) scores for each customer.
   - Segments: Champions, Loyal, Regular, At Risk.
   - Insights: Champions and Loyal drive most of the revenue.

3. **Product Strategy**
   - Identified bottom 10% low-margin SKUs.
   - Seasonal demand analysis (monthly, weekday, hourly trends).
   - Recommendation: drop low-margin SKUs, migrate demand to top-margin items.

4. **Market Basket Analysis**
   - Association rules (Apriori) for cross-sell bundles.
   - Example: *“Customers who buy Party Bunting often also buy Fairy Lights.”*

5. **Strategy Simulation**
   - Dropping low-margin SKUs + redirecting demand → **+3–6% margin uplift**.
   - Loyalty nudge for high-risk customers → **~12% relative retention uplift**.

---

## 📈 Key Insights
- **Customer Mix:** Small “Champion” group = disproportionate revenue impact.  
- **Seasonality:** Sales spike during November–December holiday season.  
- **Products:** Bottom 10% of SKUs contribute low profit despite revenue → candidates for removal.  
- **Growth Potential:**  
  - Margin uplift: **+3–6%**.  
  - Retention uplift: **~12%** relative.  

---
