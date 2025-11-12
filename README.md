# 📊 Sales Performance Analysis Dashboard (Power BI)

## 📁 Project Overview
This project focuses on analyzing **sales performance** across multiple dimensions — product, customer, promotion, and time — to uncover insights that drive business decisions.  
Using **Power BI**, I built an interactive dashboard that visualizes trends in **Sales, Profit, and Quantity Sold** from **2020 to 2024**.

---

## 🧠 Objective
To design a **data-driven Power BI dashboard** that helps stakeholders:
- Identify top and bottom performing products.
- Compare sales and profit trends across cities and time periods.
- Evaluate promotional campaign effectiveness.
- Track key business metrics (Total Sales, Total Profit, and Quantity Sold) using DAX measures.

---

## 🧩 Data Model
The project follows a **Star Schema** structure:

- **Fact Table:** Contains transaction-level sales data.  
- **Dimension Tables:**  
  - `Dim Product` – Product details (category, subcategory, etc.)  
  - `Dim Customers` – Customer information and region  
  - `Dim Promotion` – Promotional campaign details  
  - `Date Table 1` & `Date Table 2` – Custom date hierarchies for time intelligence  

---

## ⚙️ Tools & Technologies
- **Power BI** – Dashboard creation, data modeling, and visualization  
- **Microsoft Excel** – Data cleaning and preprocessing  
- **DAX (Data Analysis Expressions)** – Created calculated measures and KPIs  

---

## 📐 Key DAX Measures
```DAX
Sum of Net Sales = SUM('Fact Table'[Net Sales])
Sum of Profit = SUM('Fact Table'[Profit])
Total Quantity = SUM('Fact Table'[Quantity])
