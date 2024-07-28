# SQL-Project-on-Pizza-Sales🍕📊

This project involves analyzing pizza sales data from a database to uncover sales patterns and insights at Pizza Hut. The dataset is structured into four main tables, each capturing different aspects of pizza orders.

## Project Overview

The project aims to analyze pizza sales data to understand various sales patterns, including revenue distribution, order trends, and pizza popularity. The analysis involves querying the database to answer specific business questions and derive actionable insights.

## Dataset 📋

The dataset consists of the following tables:

1. **`order_details`**: 
   - **Columns**:
     - `order_details_id`: Unique identifier for each order detail.
     - `order_id`: Links to `orders`, identifying the order.
     - `pizza_id`: Links to `pizzas`, identifying the specific pizza.
     - `quantity`: Number of units of the pizza ordered.
   - **Purpose**: Captures details of each pizza ordered, including quantity.

2. **`orders`**:
   - **Columns**:
     - `order_id`: Unique identifier for each order.
     - `order_date`: Date of the order.
     - `order_time`: Time of the order.
   - **Purpose**: Records overall order information, including timing.

3. **`pizza_types`**:
   - **Columns**:
     - `pizza_type_id`: Unique identifier for each pizza type.
     - `name`: Name of the pizza type.
     - `category`: Category of the pizza (e.g., vegetarian).
     - `ingredients`: Ingredients used in the pizza.
   - **Purpose**: Provides details about different types of pizzas available.

4. **`pizzas`**:
   - **Columns**:
     - `pizza_type_id`: Links to `pizza_types`, identifying the pizza type.
     - `name`: Name of the specific pizza.
     - `category`: Category of the pizza.
     - `ingredients`: Ingredients used in the pizza.
   - **Purpose**: Details specific pizzas, complementing `pizza_types` with additional information.

## Analysis 🔍

The analysis includes various queries and operations to extract insights from the data:

- **Basic Analysis**: Includes queries to retrieve the total number of orders, calculate total revenue, identify the highest-priced pizza, and list the top 5 most ordered pizza types.
- **Intermediate Analysis**: Involves joining tables to find the total quantity of each pizza category ordered, analyzing order distribution by hour, and calculating category-wise pizza distribution.
- **Advanced Analysis**: Focuses on calculating the percentage contribution of each pizza type to total revenue, analyzing cumulative revenue over time, and identifying the top 3 most ordered pizza types based on revenue for each category.

## Usage 🚀

To run the analysis, follow these steps:

1. **Set Up Environment**: Ensure you have a SQL environment ready to execute the queries. You can use tools like MySQL Workbench, pgAdmin, or any other SQL client.
2. **Load Data**: Import the dataset into your SQL environment.
3. **Run Queries**: Execute the SQL queries provided to answer the questions and analyze the data.
4. **Review Results**: Review the results to gain insights into pizza sales patterns.

## Conclusion 🎉

This project demonstrates how to leverage SQL to analyze sales data and uncover meaningful patterns and trends. By querying and joining multiple tables, you can gain valuable insights into sales performance and customer preferences.

Feel free to explore, modify, and expand upon the queries to further analyze the data or adapt the project for different datasets.
