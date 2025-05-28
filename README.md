# 📊 E-Commerce Sales & Perfomance Dashboard – Power BI Project

## 📁 Project Overview

This project showcases an interactive Power BI dashboard developed to analyze and visualize key metrics from an e-commerce dataset. It includes insights into **sales performance**, **product popularity**, **customer distribution**, and **geographic trends** over time.

---

## 🎯 Objectives

- Visualize total sales and order volume
- Identify top-performing products
- Analyze quantity sold and customer distribution by country
- Track revenue trends over time
- Create an interactive and user-friendly dashboard for exploration

---

## 🧰 Tools & Technologies

- **Power BI Desktop**
- **Power Query Editor** – for cleaning and shaping the data
- **DAX** – for calculated measures and KPIs
- **Bar, Line, Pie, Map & Card visuals**

---

## 📊 Dashboard Features

- **KPI Cards**:  
  - Total Revenue  
  - Total Orders  
  - Total Customers  
  - Average Order Value

- **Trend Analysis**:  
  - Monthly revenue trends using a line chart

- **Product Insights**:  
  - Top 10 products by total revenue (bar chart)

- **Geographic Insights**:  
  - Quantity sold by country  
  - Customer distribution by country (pie chart and map)

- **Slicers & Filters**:  
  - Date filter  
  - Country filter  
  - Product filter

---

## 🧹 Data Cleaning Steps

Performed in Power Query:
- Removed rows with missing `Customer ID` or `Stock Code`
- Replaced nulls and cleaned text in `Product Description`
- Converted date formats and filtered valid transactions
- Added calculated column for `Total Price = Unit Price × Quantity`

---

## 📈 DAX Measures Created

```DAX
Total Revenue = SUM('SalesData'[TotalPrice])
Total Orders = DISTINCTCOUNT('SalesData'[InvoiceNo])
Total Customers = DISTINCTCOUNT('SalesData'[CustomerID])
Average Order Value = [Total Revenue] / [Total Orders]

## 📊 Dashboard Outcomes

This Power BI dashboard presents a comprehensive overview of e-commerce sales and customer performance. Below are the key findings derived from the analysis:

### 🔹 Overall Business Performance
- **Total Revenue:** £5M+
- **Total Customers:** 3,126
- **Total Orders:** 10,000+
- **Average Order Value:** £493.71

### 📈 Monthly Revenue Trend
- The business has shown steady revenue growth over the analyzed period (2010–2011).
- Notable revenue peaks are observed in mid to late 2011, likely due to seasonality or promotional events.

### 🏆 Top 10 Products by Sales
The most successful products based on total units sold include:
1. **White Hanging Heart T-Light Holder** – 1,034 units
2. **Regency Cake Stand** – 942 units
3. **Jumbo Bag Red Retrospot** – 918 units
4. **Party Bunting** – 727 units
5. **Lunch Bag Red Retrospot** – 704 units

> These top products indicate a preference for home decor and gift-related items among customers.

### 🌍 Country-Wise Insights
- **United Kingdom** is the largest contributor to sales:
  - **Quantity Sold:** 2.24M
  - **Customer Count:** 2.82K
- Other countries with noticeable activity include:
  - **Germany** – 0.08K customers
  - **France, Netherlands, EIRE, and Australia** – minor yet valuable contributions

### 🌐 Distribution Visuals
- **Bar Chart:** Shows the total quantity sold across countries.
- **Pie Chart:** Highlights customer distribution, with the UK forming the vast majority.

---

This dashboard allows stakeholders to identify high-performing products, track revenue trends, and understand customer distribution by geography, supporting data-dr
