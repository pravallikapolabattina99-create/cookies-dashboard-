 Cookie Business Performance Dashboard
 
Project Overview--This Power BI dashboard project provides a comprehensive analysis of cookie sales, customer insights, revenue, cost, profit, and product performance.
 The solution is designed to help business stakeholders monitor overall sales performance, customer trends, and profitability through interactive and visually meaningful dashboards.
The project consists of Executive Overview and Customer Insights pages with KPI cards, trend analysis, segmentation visuals, and slicer-based filtering.

Project Objective--
The primary objective of this dashboard is to:
Monitor total orders, revenue, cost, units sold, and profit
Analyze sales trends month-wise
Understand customer purchasing behavior
Identify high-value, medium-value, and low-value customers
Compare revenue performance by city, state, and cookie type
Support business decision-making with real-time insights

Tools used --  powerbi,dax,fliter,python

Description of Dashboard Pages--

Page 1: Executive Overview Dashboard--
This page provides a high-level summary of business performance, including total orders, revenue, cost, units sold, and profit. It also shows monthly sales trends, city-wise revenue, cookie-type performance, and product sales analysis using interactive slicers.

Page 2: Customer Insights Dashboard--
This page focuses on customer-related metrics such as total customers, revenue per customer, average order value, profit margin, and customer segmentation. It helps analyze customer behavior, top-performing customers, and state-wise revenue contribution.

Key Insights--
The dashboard highlights overall business performance through total revenue, profit, cost, and units sold KPIs.
Monthly trend analysis helps identify sales growth patterns and peak performance periods.
Customer segmentation reveals high-value, medium-value, and low-value customers, supporting targeted business strategies.
Revenue analysis by city, state, and cookie type helps identify top-performing regions and products.
Profit margin and average order value provide insights into business profitability and customer purchasing behavior.

Dashboard Screenshot--
Python 

import pandas as pd
import matplotlib.pyplot as plt

summary = dataset.groupby('Cookie Type')[['Total Revenue','Units Sold']].sum()

summary.plot(kind='bar', figsize=(8,4))
plt.title('Total Revenue and Units Sold by Cookie Type')
plt.xlabel('Cookie Type')
plt.ylabel('Values')
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()


<img width="918" height="515" alt="customer " src="https://github.com/user-attachments/assets/d8b44273-a854-48d1-ba0b-2eff3c787643" />

<img width="945" height="494" alt="executive " src="https://github.com/user-attachments/assets/03e4dd4a-fa40-4c17-85e3-bf53ae092bd5" />


