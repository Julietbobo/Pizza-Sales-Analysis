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
- Instead of doin a whole year trend analysis I did a weekly and hourly trend analysis as this would be more useful in showing days that have more sales than others

### Findings
1. Generally there is a higher preference of working from the office to working from home.
2. Wednesdays have the highest office attendance.
3. Its worth noting that on Monday the percentage of people working from home is the highest.
4. The highest number recorded of absentees due to sickness in a single day is 4 (30th May 2022) which is not a significant figure to cause an alarm.
5. There are 8 employees who have been absent from work for more than 3 days in a span of 3 months.
6. From 20th June there was very low attendance whether work from home or from the office.

### Recommendations
1. Critical office activities like meetings, team lunches etc to be held on Wednesdays where we have the highest office attendance.
2. Investigate the top 8 absent employees to find out the reason for the high rate of absenteeism.
3. Check if high absenteeism from June 20th is linked to excessive workload or burnout.
4. Encourage the employees to go on leave for high productivity and to avoid burnout. 
5. On the flip side discourage extreme taking of leave days as this causes a workforce gap and low productivity.


