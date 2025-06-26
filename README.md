# 🍕 Pizza Sales Analysis Dashboard

This project analyzes a year's worth of pizza sales data using **SQL Server**, **Excel 2019**, and **Pivot Tables** to extract key business insights. The final output is a dynamic Excel dashboard that visualizes performance indicators, sales trends, and customer preferences.

---

## 📁 Project Overview

- **Tool Stack:**  
  - SQL Server Management Studio (SSMS)  
  - Excel 2019 (Power Pivot, Charts, Slicers)  
  - CSV Dataset (48,620 rows)

- **Goal:**  
  To generate a detailed sales performance dashboard that helps the pizza company identify high-performing products, busiest periods, and revenue trends.

---

## 🛠️ Steps Performed

### 1. Database Setup (SSMS)
- Created a database: `Pizza DB`
- Imported dataset as a table: `pizza_sales` (48,620 rows)

### 2. Data Cleaning
- Fixed incorrect data types (e.g., `TINYINT ➝ INT`, dates to proper `DATE`)
- Removed unnecessary null values
- Standardized `pizza_size` values:
  - `s ➝ Regular`, `m ➝ Medium`, `l ➝ Large`, `xl ➝ X-Large`, `xxl ➝ XX-Large`

### 3. Data Processing
- Extracted `order_day` (e.g., Monday, Tuesday) from `order_date`
- Calculated all KPIs using SQL queries

### 4. Dashboard Building (Excel)
- Connected Excel to SQL Server and imported the cleaned table
- Used Pivot Tables, Charts, and Slicers to build visualizations
- Customized with interactive filters (e.g., by date/quarter)

---

## 📊 KPI Metrics Calculated

| KPI | Description |
|-----|-------------|
| 💰 **Total Revenue** | Sum of `total_price` |
| 📦 **Total Orders** | Count of distinct `order_id` |
| 🍕 **Total Pizzas Sold** | Sum of `quantity` |
| 🧾 **Average Order Value** | Revenue ÷ Total Orders |
| 📊 **Avg. Pizzas per Order** | Quantity ÷ Total Orders |

---

## 📈 Charts & Visualizations

1. **Daily Trend for Total Orders** – Bar chart (Mon–Sun)
2. **Hourly Trend for Orders** – Line chart (9 AM to 11 PM)
3. **% of Sales by Pizza Category** – Pie chart (Classic, Supreme, etc.)
4. **% of Sales by Pizza Size** – Pie chart (Regular to XX-Large)
5. **Total Pizzas Sold by Category** – Bar chart
6. **Top 5 Best Sellers** – Horizontal bar chart by pizza name
7. **Bottom 5 Worst Sellers** – Horizontal bar chart by pizza name
8. **Quarter Slicer** – Timeline filter for interactive exploration

---

## 📌 Key Business Insights

- 🗓️ **Busiest Days:** Friday and Saturday
- ⏰ **Peak Hours:** 12–1 PM and 4–8 PM
- 🧀 **Best Category:** Classic pizzas contribute most to sales
- 🍕 **Top Size:** Large pizzas drive the most revenue
- ⭐ **Top Sellers:** The Classic Deluxe Pizza, Barbecue Chicken Pizza
- ❌ **Underperformer:** The Brie Carre Pizza has lowest sales & revenue

---

## ✅ Status
🎉 **Completed**  
The project demonstrates a full-cycle BI workflow: from raw data in SQL to an interactive Excel dashboard. Suitable for presentations, interviews, or portfolio showcasing.

---

## 👤 Author

**Manisai**  
🔗 [LinkedIn](#) | 📂 [Portfolio](#)

---

## 📄 License

This project is open-source and available for learning and personal use.
