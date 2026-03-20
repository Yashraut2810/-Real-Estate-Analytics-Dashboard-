Inventory Analytics Dashboard (Power BI)
**Overview**

This project presents an interactive Inventory Analytics Dashboard built using Power BI to monitor stock levels, track inventory value, and identify low-stock items. It enables businesses to make data-driven decisions for efficient inventory management and cost optimization.

**Objective**
Track total inventory quantity and value
Monitor stock distribution across categories and items
Identify low-stock items for timely restocking
Analyze inventory trends over time

**Key Features**
**KPI Metrics**
Total Quantity – Overall stock available
Total Inventory Value – Total worth of inventory
Average Price – Mean price of items

**Visual Insights**
Inventory distribution by category (Bar Chart)
High-value items analysis (Column Chart)
Stock trends over time (Line Chart)
Low stock identification (Table with alerts)

**Interactive Filters**
Category-wise filtering
Date-based filtering
Supplier-based filtering (if available)

** Tech Stack**
Power BI – Dashboard & Visualization
DAX (Data Analysis Expressions) – Calculations & Measures
Excel – Data Source

**Key DAX Measures**
Total Quantity = SUM('Inventory (4)'[Quantity])
Total Value = 
SUMX('Inventory (4)', 
    'Inventory (4)'[Quantity] * 'Inventory (4)'[Price]
)
Avg Price = AVERAGE('Inventory (4)'[Price])
Low Stock = IF('Inventory (4)'[Quantity] < 10, "Low", "OK")

**Business Impact**
Helps businesses prevent stockouts and overstocking
Improves inventory planning and operational efficiency
Enables quick identification of high-value and low-performing items

**Future Enhancements**
Inventory demand forecasting using Machine Learning
Automated restocking recommendations
Supplier performance analysis
Integration with real-time databases
