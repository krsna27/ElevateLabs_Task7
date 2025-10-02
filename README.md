📊 Sales Data Analysis with SQLite & Python

This project demonstrates how to connect a CSV dataset to SQLite, run basic SQL queries inside Python, and visualize results using matplotlib.
It’s a simple hands-on exercise to practice working with relational databases, SQL, and Python data analysis.

🚀 Features
Loads a CSV file (online_sales.csv) into an SQLite database
Runs SQL queries using sqlite3 and pandas
Generates sales summary reports (quantity & revenue per product)
Visualizes results with bar charts in Jupyter Notebook
Clean, beginner-friendly Python code


🛠️ Tech Stack
Python 3
SQLite3 (built into Python, no setup required)
Pandas (data manipulation)
Matplotlib (data visualization)
Jupyter Notebook (for step-by-step execution)

📂 Project Structure
├── online_sales.csv       # Raw sales data (input file)
├── sales_data.db          # SQLite database (auto-created)
├── sales_analysis.ipynb   # Jupyter Notebook with code & outputs
├── sales_chart.png        # Bar chart saved from notebook
└── README.md              # Project documentation

📊 SQL Queries Used
1. Sales summary by product
SELECT product,
       SUM(boxes_shipped) AS total_qty,
       SUM(amount) AS revenue
FROM sales
GROUP BY product;

📌 Notes
The database (sales_data.db) is auto-created from online_sales.csv
You can adjust queries to analyze salesperson performance, country-wise sales, or monthly trends
Bar chart can be plotted as horizontal (barh) if product names are long

🏆 Learning Outcomes

Connecting Python to SQLite
Running SQL inside Python scripts
Using pandas for query results
Visualizing business data with matplotlib