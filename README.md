# 🛒 Superstore Sales & Profit Dashboard

## 📌 Overview

The **Superstore Dashboard** is an interactive analytics solution built to provide a comprehensive view of sales performance, profitability, customer behavior, and operational efficiency across regions, categories, segments, and time.

It leverages transactional order data, return records, and regional management information to support **data-driven business decisions**.

---

## 🎯 Objectives

The dashboard is designed to:

* Monitor **overall sales and profit performance**
* Track **return rates and customer activity**
* Identify **top-performing and underperforming products, categories, and regions**
* Analyze the **impact of discounts on profitability**
* Support **regional and managerial performance evaluation**

---

## 📊 Key KPIs

Displayed at the top of the dashboard:

* **Return Rate (%)** – Proportion of returned orders
* **Total Customers** – Unique customers
* **Region Count** – Number of active regions
* **Total Sales ($)** – Overall revenue generated
* **Total Profits ($)** – Net profit after discounts
* **Unique Orders** – Distinct order count

---

## 🗂 Data Sources & Schema

### 1️⃣ Orders Table

Contains transactional-level sales data.

**Columns:**

* Row ID
* Order ID
* Order Date
* Ship Date
* Ship Mode
* Customer ID
* Customer Name
* Segment (Consumer, Corporate, Home Office)
* Country, City, State, Postal Code, Region
* Product ID
* Category (Technology, Furniture, Office Supplies)
* Sub-Category
* Product Name
* Sales
* Quantity
* Discount
* Profit

---

### 2️⃣ Returns Table

Tracks returned orders.

**Columns:**

* Returned (Yes/No)
* Order ID

**Usage:**

* Used to calculate **Return Rate**
* Linked to the Orders table via `Order ID`

---

### 3️⃣ People Table

Maps regional responsibility.

**Columns:**

* Person (Regional Manager)
* Region

**Usage:**

* Enables **sales and profit analysis by regional managers**

---

## 📈 Dashboard Visuals & Insights

### 🔹 Sales & Profit by Person

* Compares **Total Sales vs Total Profits** per regional manager
* Highlights managerial performance and regional contribution

### 🔹 Monthly Sales & Profit Trends

* Time-series analysis showing **seasonality and growth patterns**
* Helps identify peak and low-performing months

### 🔹 Sales by Category

* Revenue contribution from Technology, Furniture, and Office Supplies

### 🔹 Profit by Category

* Reveals which categories generate the **highest margins**

### 🔹 Sales & Profit by Segment

* Compares Consumer, Corporate, and Home Office segments
* Identifies the most profitable customer segment

### 🔹 Ship Mode Distribution

* Order volume by shipping method:

  * Standard Class
  * Second Class
  * First Class
  * Same Day

### 🔹 Discount vs Profit Analysis

* Scatter plot showing how **discount levels impact profitability**
* Highlights profit erosion at higher discounts

### 🔹 Profit by Product Name

* Identifies **top and bottom-performing products**
* Supports product-level optimization decisions

---

## 🎛 Filters & Interactivity

* **Region Selector:** Central, East, South, West
* **Year Range Slider:** Enables time-based analysis
* Cross-filtering across all visuals for deep exploration

---

## 💡 Key Business Questions Answered

* Which regions and managers drive the most profit?
* How do discounts affect overall profitability?
* What products and categories should be prioritized or discontinued?
* Which shipping modes are most commonly used?
* How do sales and profits vary by customer segment?

---

## 🛠 Tools & Technologies

* **Power BI** – Data modeling, DAX calculations, and visualization
* **Star Schema Data Model** – Orders as fact table, Returns & People as dimensions

---

## 🚀 Use Cases

* Executive performance reporting
* Sales and operations planning
* Discount strategy optimization
* Product and category performance analysis
* Regional management evaluation

---

## 📎 Notes

* All monetary values are displayed in USD
* Profit figures account for applied discounts
* Dashboard supports drill-down and cross-filtering for deeper insights

---

## 📄 License

This project is licensed under the **MIT License**.
