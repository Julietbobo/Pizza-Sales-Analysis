# Pizza Sales Analysis
### Project over_view.
The project aims to analyze pizza sales and draw actionable insights that will help drive sales and increase profits

![Screenshot (35)](https://github.com/user-attachments/assets/90b37c79-1e32-4e47-ba8f-da4fc33cb0eb)

## Table of contents
1. [Data Source](#data-source)
2. [Tools](#tools)
3. [Data Preparation](#data-preparation)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Assumption](#assumption)
6. [Data Analysis](#data-analysis)
7. [Findings](#findings)
8. [Recommendations](#recommendations)

### Data Source
The data is sourced from a CSV file from a youtube channel: pizza_sales.csv.

### Tools

- Power Bi - Visualization.

### Data Preparation
- Data loading and inspection
- Determine the KPIs
  - Total revenue
  - Average price per order
  - Total pizzas sols
  - Total orders
  - Average quantity per order
- Also determine the top N pizzas by orders, revenue and quantity sold

### Data Analysis
- Creating measures for the KPIs. Below are some dax measures:
  
`Avg_Price_Per_Order = SUM('pizza_sales'[total_price]) / DISTINCTCOUNT('pizza_sales'[order_id])`

`Total orders = DISTINCTCOUNT('pizza_sales'[order_id])`

`Revenue = sum('pizza_sales'[total_price])`

### Data visualization.
- For the KPIs I used visual cards.
- Instead of doing a whole year trend analysis I did a weekly and hourly trend analysis as this would be more useful in showing days and hours that have more sales than others. For the weekly trend I used a combo chart to show revenues vs orders per day and for the hourly trend I used a line chart.
- I used a pie chart to show revenue by pizza_category and pizza_size and a funnel chart to show quantity sold by pizza category.
- For the top N pizzas by orders, revenue and quantity sold I went for a bar chart since it would result in a clean visual.

![Screenshot (39)](https://github.com/user-attachments/assets/3a6256c4-fe7e-4ac4-84c9-f6818c0b407c)

  
- In addition, I customized the tooltip to show in which pizza category the pizzas belong to.
  
![Screenshot (37) - Copy](https://github.com/user-attachments/assets/1c10872a-d905-4cb9-9ca8-4db0c1c33366)

### Findings
- Pizzas in the classic category are the highest revenue contributers at 26.91% and also ranks highest in quantity sold at 14,889.
- The large size contributed the most in terms of revenue at 45.89%.
- Thursday, Friday, Saturday and Sunday have the highest pizza sales and revenues.
- Pizza sales are highest between 11 am to 1 pm and 3 pm to 6pm.

### Recommendations
- To reduce losses make sure that the least ordered pizzas are made in small quantities.
- Give midweek offers to increase sales on Mondays, Tuesdays or Wednesdays.
- The XXL size can be done away with since only 28 were sold within the whole year and it contributed less than 2% to the revenue. This will help reduce unecessary costs.

