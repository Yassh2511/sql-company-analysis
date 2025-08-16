# Walmart Sales Data Analysis  

## 📌 Overview  
This project analyzes Walmart sales data to understand:  
- Which products and branches perform best  
- Sales trends across days, months, and time of day  
- Customer behavior and spending patterns  
- Which customer segments generate more revenue  

The dataset comes from the [Kaggle Walmart Sales Forecasting Competition](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting).  

---

## 📊 Dataset  
The dataset contains transactions from 3 Walmart branches located in **Mandalay, Yangon, and Naypyitaw**.  
It has **1000 rows and 17 columns** including:  

- `invoice_id` → Unique sales invoice  
- `branch`, `city` → Store details  
- `customer_type`, `gender` → Customer information  
- `product_line` → Product category  
- `unit_price`, `quantity`, `cogs`, `VAT`, `total`, `gross_income` → Financial details  
- `date`, `time` → Transaction timestamp  
- `payment` → Payment method  
- `rating` → Customer feedback  

---

## 🔎 What I Did  

1. **Data Cleaning**  
   - Checked for missing/null values (none found).  

2. **Feature Engineering**  
   - Added `time_of_day` (Morning, Afternoon, Evening).  
   - Extracted `day_name` (Mon–Sun).  
   - Extracted `month_name` (Jan–Dec).  

3. **Exploratory Data Analysis (EDA)**  
   - Analyzed top product lines and branches.  
   - Compared revenue across months and days.  
   - Studied customer types, gender distribution, and payment methods.  
   - Checked customer ratings by day and branch.  

4. **Revenue & Profit Calculations**  
   - `COGS = unit_price * quantity`  
   - `VAT = 5% * COGS`  
   - `total = COGS + VAT`  
   - `gross_income = total - COGS`  
   - `gross_margin = gross_income / total`  

---

## ❓ Key Questions Answered  
- Which product lines sell the most?  
- Which city/branch generates the highest revenue?  
- What is the most common payment method?  
- Do members or normal customers spend more?  
- Who buys more: male or female customers?  
- Which days and times see the highest sales?  
- Which branches get the best ratings?  

---

## 🛠 Tools & Technologies  
- **SQL** → Queries and analysis  
- **Python (Pandas, Matplotlib, Seaborn)** → Data exploration & visualization  

---

## ✅ Conclusion  
The analysis provided insights into product performance, branch revenue, customer behavior, and sales patterns.  
These findings can help improve sales strategies, optimize product offerings, and better target customer segments.  
