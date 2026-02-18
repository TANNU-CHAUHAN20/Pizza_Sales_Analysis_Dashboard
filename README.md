# Pizza_Sales_Analysis_Dashboard
Power BI Dashboard 
# Project Objective
To analyze pizza sales data to identify key business insights such as revenue trends, best-selling products, customer preferences, and sales performance across different categories, using data analysis tools to support data-driven decision making.
# Project Insights
Designed an interactive sales dashboard to analyze pizza performance using transactional data.
 Visualized top & bottom-selling pizzas based on revenue and quantity sold.
 Analyzed revenue distribution by category and size to identify customer purchasing patterns.
 Tracked total sales trends across weekdays to optimize demand forecasting.
 Enabled data-driven insights to improve product strategy and sales performance.
Top 5 pizzas contribute nearly 40–50% of total revenue.
#Dax Queres
1.Total Sold Quantity = FORMAT(sum(pizza_sales[quantity]),"##,###")
2..weekday = WEEKDAY(pizza_sales[order_date],1)
3.Weekday Name = FORMAT(WEEKDAY(pizza_sales[order_date],1),"ddd")
4.Total Orders = count(pizza_sales[order_date])
5.Total Quantity = sum(pizza_sales[quantity])
6.Total Sales = sum(pizza_sales[total_price])
7.Parameter = {
    ("Total Orders", NAMEOF('Table'[Total Orders]), 0),
    ("Total Quantity", NAMEOF('Table'[Total Quantity]), 1),
    ("Total Sales", NAMEOF('Table'[Total Sales]), 2)
}
