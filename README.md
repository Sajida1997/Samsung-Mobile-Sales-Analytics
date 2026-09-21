# 📊 Samsung Mobile Sales Analytics Dashboard

## Overview
This project showcases a Power BI dashboard analyzing mobile sales performance across multiple brands, models, cities, payment methods, and customer ratings.  
The goal is to demonstrate **data visualization, DAX calculations, and business insights** for decision-making.

---

## Key Features
- **KPIs:** Total Sales, Quantity, Transactions, Average Price
- **Geographic Analysis:** Sales by city (Chennai, Madurai, Bangalore)
- **Trend Analysis:** Quantity sold by month and day of week
- **Customer Insights:** Ratings distribution (1–5 stars)
- **Payment Trends:** UPI, Debit Card, Cash, Credit Card split
- **Brand Performance:** Samsung, OnePlus, Vivo, Xiaomi comparison
- **Model Comparison:** iPhone SE, OnePlus Nord, Galaxy Note 20

---

## Visuals Used
- **KPI Cards** → Quick performance indicators  
- **Map** → Regional sales distribution  
- **Line Charts** → Trends over time (monthly, weekly)  
- **Bar Chart** → Customer ratings comparison  
- **Pie Chart** → Payment method share  
- **Table** → Brand breakdown  
- **Column Chart** → Model sales comparison  

👉 Each visual was chosen to highlight **clarity, comparability, and actionable insights**.

---

## DAX Formulas
Some of the measures applied in this dashboard:

```DAX
Total Sales = SUM(Sales[Amount])
Total Quantity = SUM(Sales[Quantity])
Total Transactions = COUNTROWS(Sales)
Average Price = DIVIDE([Total Sales], [Total Quantity])
Sales by Day = CALCULATE([Total Sales], VALUES(Sales[DayName]))
