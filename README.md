# 📘 README: Subqueries in WHERE Clause – MySQL Tutorial

##📌 Project Title:
Advanced SQL Queries: Subqueries in the WHERE Clause

## 📝 Description
This notebook explores advanced SQL querying techniques, focusing specifically on **subqueries within the WHERE clause**. The tutorial leverages the `united_nations` MySQL database, which includes tables such as:

  - `Access_to_Basic_Services`
  
  - `Economic_Indicators`
  
  - `Geographic_Locations`

The main objective is to demonstrate how subqueries can compare individual row data to **aggregated results**, filter complex datasets, and answer real-world questions about development indicators across countries.

##b🎯 Learning Objectives
By completing this notebook, users will be able to:

  - Understand how subqueries function in the `WHERE` clause.
  
  - Write queries that compare values against subquery results (e.g., `> (SELECT AVG(...))`).
  
  - Join multiple tables in subqueries for richer insights.
  
  - Filter data using nested queries and logical conditions.

## ⚙️ Requirements
- Local installation of MySQL Workbench

- MySQL Server running locally with:

    - Database: `united_nations`
    
    - Tables: `Basic_Services`, `Economic_Indicators`, `Geographic_Locations`

- Python environment with:

  - `SQLAlchemy`
  
  - `pymysql`
  
  - Jupyter Notebook or VS Code

## 🔌 Database Connection
Ensure that the MySQL server is running locally and accessible through this connection string:
```
mysql+pymysql://root:<your_password>@localhost:3306/united_nations
```
| ❗ Google Colab will not work with this tutorial as it cannot connect to your local MySQL instance.

## 📂 Dataset Overview
`Access_to_Basic_Services`
  - `Country_name`
  
  - `Year`
  
  - `Water_access_pct`
  
  - `Electricity_access_pct`
  
  - ...

`Economic_Indicators`
  - `Country_name`
  
  - `Time_period`
  
  - `Est_gdp_in_billions`
  
  - `Est_population_in_millions`
  
  - `Pct_unemployment`
  
  - ...
`Geographic_Locations`
  - `Country_name`
  
  - `Region`
  
  - `Continent`
  
  - ...

## 📊 Sample Use Cases Explored
  - Countries with above-average GDP but below-average water access
  
  - Countries where unemployment is higher than the global average
  
  - Comparing a country's population to the average population of its region
  
  - Filtering records based on values returned from aggregated subqueries

## 🚀 How to Run
  1. Clone this project locally.
  
  2. Set up the `united_nations` MySQL database and import the required tables.
  
  3. Launch the notebook in Jupyter or your preferred IDE.
  
  4. Run each cell sequentially after ensuring the database connection is active.

## 📁 File Structure
```
├── sql_subqueries_where.ipynb        # Main tutorial notebook
├── README.md                         # Project overview and guide
├── data/                             # (Optional) CSVs used to seed the DB
└── queries/                          # Saved SQL scripts (if applicable)
```

## 🧠 Author Notes
This tutorial is part of a broader training on data-driven decision making using SQL. It builds on previous lessons covering:

  - Aggregate functions
  
  - GROUP BY and HAVING
  
  - Subqueries in FROM

If you're following the full course, ensure your MySQL setup includes all required schema and data.

## 📧 Contact
For questions, reach out to:

Name: Ibrahim Ambale

LinkedIn: [Ibrahim Ambale](https://www.linkedin.com/in/ibrahim-ambale/)
