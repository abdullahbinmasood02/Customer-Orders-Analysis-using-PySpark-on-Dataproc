# Customer & Orders Analysis using PySpark on Dataproc

This project demonstrates a customer and orders analysis using PySpark on a Google Dataproc cluster. The datasets used are:

- `customers.csv` — customer information
- `orders.csv` — order details

The goal is to clean, transform, and analyze the data to get actionable business insights.

---

## Project Steps

### 1. Customer Data Processing

- Read the customer CSV dataset.
- Converted `reg_date` to date type.
- Converted `is_active` to Boolean.
- Filled missing values for key columns with 'unknown'.
- Extracted registration year and month as separate columns.
- Counted unique cities, states, and countries.
- Calculated the number of customers per city, state, and country.
- Counted active and inactive customers per state.
- Identified recent customers based on registration date.
- Found the oldest and newest customer per city.
- Saved the cleaned and processed customer data as a Parquet file.

### 2. Orders Data Processing

- Joined customers and orders datasets.
- Calculated total orders by customer and ordered by descending count.
- Calculated total spend by customer and ordered by descending spend.
- Found average spend per customer.
- Determined order status grouped by customer.
- Analyzed orders grouped and ordered by month.

---

The project provides insights into customer behavior and order patterns, helping to identify high-frequency but low-spend customers and enabling data-driven business decisions.