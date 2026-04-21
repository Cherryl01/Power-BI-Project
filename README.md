# 📊 Ultra Packaged Store – Power BI Sales Analytics Dashboard

## 🔷 Project Overview
This project presents an interactive **Power BI dashboard** built to analyze the performance of a retail (beauty/packaged store) business. It focuses on **sales, customers, and product performance**, transforming raw data into actionable business insights.

The dashboard enables stakeholders to:
- Monitor revenue and sales trends  
- Understand customer behavior  
- Identify top-performing products and regions  
- Support data-driven decision-making  

---

## 🖼️ Dashboard Preview

### 🔹 Main Dashboard
![Main Dashboard](https://github.com/Cherryl01/Power-BI-Project/blob/main/Images/Main%20Dashboard.png)

### 🔹 Overview Dashboard
![Overview Dashboard](https://github.com/Cherryl01/Power-BI-Project/blob/main/Images/dashboard%20overview.png)

---

## 🔷 Key Metrics (KPIs)

The dashboard highlights important business metrics:

- 💰 **Total Revenue:** 29M  
- 🧾 **Total Orders:** 28K  
- 👥 **Total Customers:** 18K  
- 📊 **Average Order Value:** 1.06K  

---

## 🔷 Features & Analysis

### 📈 Sales Analysis
- Revenue trends across time  
- Sales distribution by country  
- Category-level performance  

### 👥 Customer Insights
- Revenue per customer  
- Customer lifetime value (CLV)  
- Customer distribution by region  
- Repeat vs new customer behavior  

### 🛍️ Product Performance
- Top-selling products  
- Category performance (Bikes, Clothing, Accessories)  
- Quantity sold per product  
- Identification of low-performing items  

---

## 🔷 Data Model

The project is built using a **relational data model**:

### Fact Table:
- `fact_sales` (sales transactions)

### Dimension Tables:
- `dim_customers`
- `dim_products`

### Relationships:
- `product_id` → connects sales to products  
- `customer_id` → connects sales to customers  

---

## 🔷 Key DAX Measures

```DAX
Total Revenue = SUM('fact_sales'[sales_amount])

Total Orders = COUNT('fact_sales'[order_id])

Average Order Value = DIVIDE([Total Revenue], [Total Orders])
