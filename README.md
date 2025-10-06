
# 🟦 Sales Performance Analysis Project

## 📌 Project Overview
This project focuses on analyzing **sales performance**, **customer behavior**, and **product trends** using **SQL** for data exploration and transformation, followed by **Power BI** for visualization.

The goal was to perform end-to-end analysis starting from **raw Excel data → SQL exploration & cleaning → creating aggregated views → building interactive dashboards**.

---

## 📊 Data Sources
The analysis was based on three Excel sheets:

- **fact_sales.xlsx** → Contains transactional data (orders, sales amount, quantity, date)  
- **dim_customers.xlsx** → Customer demographic and profile data  
- **dim_products.xlsx** → Product details including category, subcategory, and cost

These sheets were loaded into a SQL database for processing and analysis.

---

## 🧪 SQL Exploratory Data Analysis (EDA)
I performed extensive SQL EDA to understand the dataset, including:

- Exploring **countries**, **product categories**, and **customer demographics**  
- Calculating key business metrics:
  - Total sales, total quantity sold, average selling price  
  - Number of orders, products, and customers  
- Identifying **top products** and **top customers** by revenue  
- Analyzing **sales trends over time** (monthly and yearly)  
- Segmenting products by **cost ranges** and **performance**  
- Segmenting customers by **spending behavior** and **lifespan**:
  - **VIP**: Lifespan ≥ 12 months and total sales > 5,000  
  - **Regular**: Lifespan ≥ 12 months and total sales ≤ 5,000  
  - **New**: Lifespan < 12 months

---

## 🏗️ SQL Views Creation
To prepare clean and analytical datasets for visualization, I created two key SQL views:

### `gold.customer_report`
- Aggregates **customer-level metrics** (total orders, products, sales, quantity, lifespan, recency)  
- Segments customers by **age group** and **value (VIP, Regular, New)**

### `gold.product_report`
- Aggregates **product-level performance metrics**  
- Includes KPIs like **lifespan**, **total customers**, **AOV**, and **performance segmentation (High, Mid, Low)**

These views make it easy to connect analytical tools and avoid complex calculations inside Power BI.

---

## 📈 Power BI Dashboards
After preparing the SQL views, I connected Power BI directly to the SQL database to load the `gold.customer_report` and `gold.product_report` views.

Using these clean and aggregated views, I built three interactive dashboards to visualize key business insights:

### 🟦 Overview Dashboard
- Total Revenue, Orders, Quantity, AOV, and overall performance trends

### 🟨 Customers Dashboard
- Customer segmentation by age, gender, country  
- Revenue breakdown by customer segment (VIP / Regular / New)  
- Top customers analysis

### 🟩 Products Dashboard
- Revenue by category and subcategory  
- Product performance segments (High, Mid, Low)  
- KPIs like lifespan and recency

---

## 📝 Key Insights
- Revenue grew strongly until **2013**, then dropped sharply in **2014** (data gap or business issue)  
- **VIP and Regular customers** contribute over **70% of revenue**  
- **Bikes** category dominates sales (~95%), with **Road** and **Mountain bikes** leading  
- **USA** and **Australia** are the top markets  
- High **AOV (1K+)** indicates high-value transactions

---

## 🧠 Recommendations
- Launch **loyalty programs** for VIP customers to maintain their engagement  
- Invest in **Accessories and Clothing** to diversify revenue streams  
- Target **marketing campaigns in Europe** (UK, Germany, France) to grow underperforming regions  
- Encourage **new customers** to make repeat purchases through offers and cross-selling strategies

---

## 🧰 Tools & Technologies
- 📝 **Excel** → Initial data source  
- 🧪 **SQL** → EDA, transformation, and view creation  
- 📊 **Power BI** → Dashboards and visualization

---

## 👤 Author
**Nabil Mohammed**  
🔗 [GitHub](https://github.com/nabilmo27)
