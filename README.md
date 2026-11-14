# Python Data Analysis Projects

Exploratory data analysis (EDA) projects built in Jupyter Notebook, covering data cleaning, aggregation, visualization and business insights.

**Libraries:** Python, Pandas, NumPy, Matplotlib, Seaborn

| # | Project | Domain | Data size | Files |
|---|---------|--------|-----------|-------|
| 1 | Cafe Sales Analysis | Food & Beverage | 1,000 orders, 26 columns | `Cafe.ipynb`, `Cafe.csv` |
| 2 | Walmart Sales Analysis | Retail | 5,000 transactions, 28 columns | `Walmaart.ipynb`, `Walmart.csv`, `Cleaned_Walmart_Data.csv` |
| 3 | Diwali Sales Analysis | Retail / E-commerce | 15,000 orders, 14 columns | `Diwali_Sales_Analysis.ipynb`, `Diwali_Dashboard_2.csv` |

---

## 1. Cafe Sales Analysis
**Data:** `Cafe.csv` | 1,000 orders, Jan-Jun 2025, 6 cities, 4 branches, 15 menu items

**Business question:** Which menu items, categories, branches and cities drive revenue, and how do customers pay and rate their orders?

**What the notebook does**
- Data checks: shape, data types, missing values, statistical summary.
- KPIs: total revenue, average bill, maximum bill.
- Charts: top-selling menu items, sales by category, payment method usage, customer type, monthly revenue trend, city and branch revenue, rating distribution, weekend vs weekday orders, bill amount vs loyalty points, category by gender.

**Key findings**
- Total revenue of ₹8.51 lakh, average bill ₹851.
- **Beverage** contributes 41.8% of revenue, Food 38.0% and Dessert 20.2%.
- **Pizza** is the top revenue item (12.9%), and the 10 largest bills are all Pizza orders. **Latte** is the most sold item by quantity.
- **Urban Brew** is the best branch (27.1% of revenue) and **Cafe Bliss** the lowest (20.9%). Nagpur and Latur lead among cities (about 17% each).
- Payment methods are evenly split (UPI 33.5%, Card 33.3%, Cash 33.2%).
- Monthly revenue was lowest in February (₹1.11 lakh) and highest in June (₹1.68 lakh).

---

## 2. Walmart Sales Analysis
**Data:** `Walmart.csv` (raw) and `Cleaned_Walmart_Data.csv` (output of the notebook) | 5,000 transactions, 3,848 customers, 5 stores, 8 products (Jan-Sep 2024)

**Business question:** Which categories, products and stores generate the most revenue, does running a promotion increase sales, and how reliable are inventory and demand forecasts?

**What the notebook does**
- Data cleaning: converted the transaction date to datetime, created a `Revenue` column (`quantity_sold` x `unit_price`), handled missing values in `promotion_type`.
- Charts: top categories, monthly revenue trend, customer gender distribution, revenue by store location, quantity sold distribution, promotion impact, top 10 products, stockout rate by store, forecasted vs actual demand.
- Exported the cleaned dataset to `Cleaned_Walmart_Data.csv`.

**Key findings**
- Total revenue of about 15.26M across 5,000 transactions.
- **Electronics** (52%) and **Appliances** (48%) are almost equal in revenue.
- **Los Angeles** is the top store (21.5%); the 5 stores are within 19-21.5% of each other.
- Top products by revenue: **TV** (2.05M), **Tablet** (2.00M) and **Fridge** (1.94M).
- Transactions with a promotion average 3,093 in revenue vs 3,009 without, a difference of only about 2.8%.
- **Stockouts** occur in about 52% of transactions (51.9%), a major inventory risk.
- The demand forecast is off by about 137 units on average, roughly 46% of average demand, so forecasting needs improvement.

---

## 3. Diwali Sales Analysis
**Data:** `Diwali_Dashboard_2.csv` | 15,000 orders, 7,259 customers, 28 states (2025)

**Business question:** How do sales vary across categories, payment methods, states and months, and how healthy is order fulfilment?

**What the notebook does**
- Data checks: missing values, duplicates, and validation that `Total_Sales_INR` equals `Quantity` x `Unit_Price_INR` (100% match).
- KPIs: revenue, orders, customers, average order value, average rating.
- Charts: revenue by category, payment-method share, orders by delivery status, return rate by category, monthly revenue trend, top 10 states, top 10 products, rating distribution.

**Key findings**
- Total revenue of Rs 111.8 Cr, average order value Rs 74.5K.
- Revenue is spread almost evenly across the 5 categories (19.4-20.3% each) and 4 payment methods (about 24-26% each).
- Only 33.8% of orders are delivered; **32.5% are returned** and **33.6% are pending**, a major fulfilment risk.
- Monthly revenue stays within Rs 8.5-9.8 Cr (lowest in February, highest in August) with no festive-season spike.
- Average rating is 3.04 and nearly identical across categories and delivery statuses.

---

## How to run
1. Install the libraries: `pip install -r requirements.txt`
2. Download the notebook and its CSV file into the same folder.
3. Open the notebook with `jupyter notebook` and run all cells.

## About me
**Shivtej Chougule**, aspiring Data Analyst (SQL, Excel, Power BI, Python).
[LinkedIn](https://www.linkedin.com/in/shivtej-chougule-723360414) | shivtejchougule16@gmail.com | [Power BI Dashboards](https://github.com/shivtejchougule16/PowerBiDashboards)
