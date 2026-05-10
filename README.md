# 📊 Sales Dashboard - Power BI Project

## 📌 Project Overview

This project is an end-to-end Sales Analytics Dashboard built using Power BI to analyze sales performance, profit, orders, and profit margin. The dashboard provides year-over-year comparisons and interactive insights across products, customers, cities, and sales channels.

## 🎯 Business Objective

The goal of this dashboard is to help businesses monitor key sales KPIs, identify trends, and make data-driven decisions by analyzing performance across multiple dimensions.

## 📈 Key KPIs

* Total Sales
* Total Profit
* Total Orders
* Profit Margin %
* Products Sold

## 🧮 DAX Measures Used

```DAX
Sales = SUM(Sales_Data[Sales])

Sales PY = CALCULATE([Sales], SAMEPERIODLASTYEAR(DateTable[Date]))

Sales vs PY = [Sales] - [Sales PY]

Sales vs PY % = DIVIDE([Sales vs PY], [Sales], 0)

Products Sold = SUM(Sales_Data[Order Quantity])

Profit = SUM(Sales_Data[Profit])

Profit LY = CALCULATE([Profit], SAMEPERIODLASTYEAR(DateTable[Date]))

Profit Vs LY = [Profit] - [Profit LY]

Profit vs LY % = DIVIDE([Profit Vs LY], [Profit], 0)

Profit Margin = DIVIDE([Profit], [Sales], 0)

Total Cost = SUM(Sales_Data[Total Cost])
```

## 📊 Dashboard Features

* Sales by Product with previous year comparison
* Monthly Sales trend analysis
* Top 5 Cities by Sales
* Profit by Sales Channel
* Customer Sales analysis
* Interactive slicers for Date, City, Product, and Channel

## 🛠️ Tools & Technologies

* Power BI Desktop
* Power Query
* DAX
* Data Modeling
* Time Intelligence Functions

  
## 📌 Key Insights

* Analyze year-over-year sales and profit performance
* Identify top-performing products and customers
* Discover the most profitable sales channels
* Track sales trends across cities and time periods

## 📂 Project Structure

```text
Sales-Dashboard-PowerBI/
├── Sales_Dashboard.pbix
├── Sales_Data.xlsx
├── README.md
└── screenshots/
    ├── dashboard-overview.png
    └── sales-analysis.png
```

## 🚀 How to Use

1. Download the `.pbix` file.
2. Open it in Power BI Desktop.
3. Refresh the data if needed.
4. Interact with slicers and visuals to explore insights.

## 👩‍💻 Author

Aya Ali
