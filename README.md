# 🛍 Retail Data Analysis – Databricks & PySpark

## 📘 Project Overview
This project focuses on Retail Data Analysis using Databricks and PySpark.  
It connects to Azure Data Lake Storage, loads multiple datasets, performs ETL transformations, and creates interactive dashboards powered by **Gold tables.  

The goal is to build an end-to-end data pipeline that delivers actionable business insights across sales, customers, stores, and product performance.

---

## ⚙ Datasets & Architecture
![Databricks](https://github.com/iouhyt6e54as/databricks--PowerBi/blob/main/images/databricks.jpg?raw=true)

### Source Data (Bronze Layer)
The following datasets are loaded from Azure Data Lake (Parquet files):
- Products
- Transactions
- Stores
- Customers

Bronze Layer:  
Raw data is loaded and stored in Databricks tables (e.g., products_bronze, transactions_bronze).

Gold Layer:  
Transformed, aggregated, and business-ready data stored for reporting and dashboard visualization.

---

## 📊 Dashboard Pages (Power BI / Databricks Visualization)

### 🟩 Page 1 – Executive Overview
![Executive Overview](images/image%201.jpg)
Purpose:  
Summarize overall business performance through key KPIs and sales trends.

Visuals:
- KPI Cards: Total Revenue, Quantity Sold, Transactions, Unique Customers, Average Order Value (AOV)
- Line Chart: Monthly revenue by year (monthly_sales_gold)
- Bar Chart: Sales by country (sales_by_country_gold)
- Stacked Column Chart: Revenue by price segment & category (price_segment_analysis_gold)
- Donut Chart: Category revenue contribution (product_performance_gold)

Outcome:  
A clean, professional dashboard delivering actionable insights into:
- Market performance  
- Customer behavior  
- Store & product profitability  
- Seasonal and geographic sales patterns  

🧠 Insight: Tracks company growth, market comparison, and category revenue distribution.

---

### 🟦 Page 2 – Customer & Market Insights
![Customer & Market Insights](images/image%202.jpg)
Purpose:  
Explore customer registration, product affinity, and geographic trends.

Visuals:
- Line Chart: Customer registration trend (customer_registration_trends_gold)
- Map: Revenue & customers by country (country_detailed_analysis_gold)
- Table: Customer–Product affinity (customer_product_affinity_gold)
- Clustered Column Chart: Category revenue by country (category_country_performance_gold)

🧠 Insight: Reveals customer loyalty, market strength, and product interest per region.

---

### 🟨 Page 3 – Store & Product Performance
![Store & Product Performance](images/image%203.jpg)
Purpose:  
Evaluate store performance, seasonal patterns, and product efficiency.

Visuals:
- Table: Store metrics (transactions, customers, avg. per customer)
- Bar Chart: Store revenue by product (store_product_performance_gold)
- Matrix: Seasonal revenue by category (seasonal_analysis_gold)
- Scatter Chart: Product performance (product_performance_gold)

🧠 Insight: Identifies top-performing stores, seasonal sales peaks, and customer engagement patterns.

---

## 🧱 Notebook Technical Workflow
![Technical Workflow](images/project%20pipline.jpg.png)

### 1. Welcome Message
Ensures that the Databricks environment is active.

### 2. Azure Data Lake Connection
Configures Spark credentials to securely access Azure Data Lake Storage.

### 3. Load Datasets
Loads Parquet files into Spark DataFrames:
- df_products
- df_transactions
- df_stores
- df_customers

### 4. Bronze Tables Creation
Raw data saved into Databricks under the schema shahdfarghaly.sales (e.g., *_bronze).

### 5. Data Transformation
Intermediate cleaning and transformation steps prepare the data for analytics.

### 6. Gold Tables Creation
Aggregated and business-ready tables (*_gold) are created for visualization in Power BI or Databricks dashboards.

---

## 🧾 Summary
This project represents a complete data engineering and analytics pipeline, including:
- Data ingestion from Azure Data Lake  
- ETL processing using PySpark  
- Data modeling through Bronze and Gold layers  
- Interactive Power BI dashboards  

📊 Outcome:  
A scalable, professional data solution delivering insights on:
- Sales trends  
- Market performance  
- Customer behavior  
- Store and product efficiency  

---

## 🧑‍💻 Tools & Technologies
- Databricks
- PySpark
- Azure Data Lake Storage (ADLS)
- Power BI / Databricks Visualization
- SQL
- Python

---

## 👩‍💼 Author
Shahd Ahmed Farghaly  
Data Science Student – Alexandria University  
📧 shahdfarghaly2005@gmail.com 
🔗 [LinkedIn Profile](www.linkedin.com/in/shahd-farghaly-bb9356332)



