# Mobile_Sales_Dashboard
📱 Mobile Sales Report

This repository contains the Power BI report Mobile Sales Report, designed to provide detailed insights into mobile device sales across various dimensions such as product, region, and time.

📄 Project Overview

The Mobile Sales Report aims to:

    Analyze sales performance by device, region, and sales period

    Identify top-selling models and underperforming products

    Visualize sales trends, sales volume, and customer ratings

    Provide actionable insights for sales and marketing teams

    📁 Files
File	                                                     Description
`Mobile_sales_report.pbix`	-                            Power BI file containing all data models, visualizations, and report pages.
`Mobile_sales_report.pdf`   -                            PDF file containing the dashboard pages
`Mobile-Sales-Performance-Tracking-and-Analysis.ppt` -   PPT file containing the summary report 
`Mobile Sales Data.xlsx`    -                            Excel file containig the sales dataset

🚀 Key Features

    Interactive Dashboards: Filterable reports by brand, region, month, and more

    Sales KPIs: Revenue, units sold, profit margins

    Top Product Analysis: Best and worst-performing devices

    Time-Series Analysis: Sales trends over time

    Regional Insights: Sales distribution across regions

🛠️ Tools and Technologies

    Power BI Desktop

    DAX (Data Analysis Expressions)

    Power Query Editor

    Data Modeling (relationships between Mob_sales and Custom_calendar tables)

🧮 DAX Formulas Used

    `MTD = TOTALMTD([Total_sales],Custom_calendar[Date].[Date])`
    
    `Same Period Last Year = CALCULATE([Total_sales],SAMEPERIODLASTYEAR(Custom_calendar[Date].[Date]))`
    
    `Total_quantity = SUM(Mob_sales[Units Sold]) `
    
    `Total_sales = SUMX(Mob_sales, Mob_sales[Units Sold] * Mob_sales[Price Per Unit])`
    
    `Transaction = COUNTROWS(Mob_sales)`

📊 Data Sources
    
    Mobile Sales Dataset from Kaggle dataset

📝 Usage

    Open the .pbix file with Power BI Desktop.

    Refresh data (if connected to live sources).

    Interact with slicers and filters to explore different insights.

    Customize visualizations if needed based on your organization's requirements.

📌 Requirements

    Power BI Desktop 
