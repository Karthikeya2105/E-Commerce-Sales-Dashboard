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
