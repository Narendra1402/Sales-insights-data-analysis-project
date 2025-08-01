
# 📊 Sales & Profit Analysis Dashboard

A comprehensive Power BI project powered by SQL Server that provides in-depth analysis of sales performance, revenue contribution, and profitability across different markets, products, and customers. This dashboard empowers business stakeholders to make data-driven decisions by understanding revenue trends, market potential, and profit drivers.



## 🚀 Problem Overview

The company operates across multiple markets and sells a wide range of products through various customers. However, they lacked a unified system to:

- Monitor sales and profit metrics in real time.
- Identify high and low-performing markets and products.
- Analyze profitability by region, product, and customer.
- Track revenue contribution, trends, and profit margins over time.

This Power BI dashboard solves the above problems by connecting directly to a SQL Server database, transforming the data, and visualizing insights across three key analytical dashboards.



## 🧩 Tools & Technologies Used

- **Power BI Desktop** – For data visualization and dashboard creation.
- **SQL Server** – For querying and fetching data into Power BI.
- **DAX** – Used in Power BI to create calculated columns, KPIs, and custom measures.
- **Power Query** – For ETL operations (data cleaning, shaping, and transformation).



## 🔗 Data Connectivity & Structure

- Connected Power BI to SQL Server using DirectQuery mode.
- Imported tables: `Sales`, `Customer`, `Market`, `Product`, `Profit`.
- Relationships were defined in a star schema for efficient querying.



## 📈 Dashboards Overview

### 1. **Sales Analytics Dashboard**

📌 **Objective:** Get a quick overview of revenue, total sales quantity, and profit margin.
<img width="884" height="556" alt="Capture6" src="https://github.com/user-attachments/assets/2a293a87-7db8-4309-9207-f5462991f8e2" />

**Key Highlights:**

- **Revenue by Market:** Delhi NCR, Mumbai, and Ahmedabad are top-performing regions.
- **Sales Quantity by Market:** Delhi NCR leads with nearly 1M units sold.
- **Top 5 Customers & Products:** Identify your most valuable customers and best-selling products.
- **Revenue Trend:** View monthly revenue growth from 2018 to 2020.



### 2. **Profit Analysis Dashboard**

📌 **Objective:** Understand how profit is distributed across markets and customers.
<img width="885" height="550" alt="Capture7" src="https://github.com/user-attachments/assets/2b4b5dde-6092-4fa1-9cb4-54665cfb0fdf" />

**Key Highlights:**

- **Revenue & Profit Contribution % by Market:** Delhi NCR contributes ~55% to revenue, while Mumbai contributes ~24% to profits.
- **Profit % by Market:** Highlights both profitable and loss-making regions.
- **Customer Profitability Table:** View detailed metrics like revenue, profit margin %, and profit amount for each customer.
- **Monthly Revenue Trend (2020):** Understand revenue and margin movements over the first 6 months of 2020.



### 3. **Performance Insight Dashboard**

📌 **Objective:** Measure how well each market and customer performs against targets.
<img width="881" height="553" alt="Capture8" src="https://github.com/user-attachments/assets/8a97e686-7103-4f40-acf1-44a35964ec66" />


**Key Highlights:**

- **Revenue Contribution vs Target %:** Highlights markets exceeding or falling short of their contribution benchmarks.
- **Combined Trend of Revenue, Revenue LY (Last Year), and Profit %:** Evaluate growth and profitability over time.
- **Customer Profitability Table (Extended):** Includes deeper metrics like total sales quantity and target comparisons.



## 🛠️ Implementation Steps

1. **Data Modeling:**
   - Connected Power BI to SQL Server.
   - Imported raw tables and created relationships between them.
   - Applied necessary data transformations using Power Query.

2. **DAX Measures:**
   - `Total Revenue = SUM(Sales[Revenue])`
   - `Total Profit = SUM(Profit[Amount])`
   - `Profit Margin % = [Total Profit] / [Total Revenue]`
   - `Revenue LY = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(Date[Date]))`

3. **Report Pages:**
   - Designed separate pages for Sales, Profit, and Performance Insight.
   - Used slicers for filtering by **Year** and **Month**.
   - Added KPI cards, bar charts, line graphs, and tables for insight delivery.



## 🎯 Key Insights & Outcomes

- **Top Customer:** Electricalsara Stores contributes over ₹65M in revenue.
- **Top Market:** Delhi NCR consistently dominates in both sales volume and revenue.
- **Market Risk:** Cities like Lucknow and Kanpur contribute negatively or very low, indicating areas of concern.
- **Product Performance:** Few SKUs like `Prod040` and `Prod159` bring high revenue, suggesting areas to scale.



## 📁 Folder Structure (If Packaged)

```
📦Sales-Profit-Analysis
 ┣ 📁SQL Scripts
 ┃ ┗ 📄Data_Import_Query.sql
 ┣ 📁Power BI
 ┃ ┗ 📄Sales_Profit_Dashboard.pbix
 ┣ 📁Images
 ┃ ┣ 📄Sales_Analytics.png
 ┃ ┣ 📄Profit_Analysis.png
 ┃ ┗ 📄Performance_Insight.png
 ┗ 📄README.md
```



## 📌 Conclusion

This project demonstrates how combining **Power BI** with **SQL** can unlock powerful sales and profit insights for businesses. It not only provides a birds-eye view of the company’s financial health but also guides targeted action for growth and efficiency.



## 🔗 Connect With Me  
Feel free to explore more of my projects and reach out:  
- [LinkedIn](https://www.linkedin.com/in/narendrasingh1402)
- [YouTube](https://www.youtube.com/@Analyst_Hive)  
- [Portfolio](https://narendra1402.github.io/)
