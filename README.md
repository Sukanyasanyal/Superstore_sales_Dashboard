# Superstore Sales Financial Performance Dashboard

##Project Goal: To analyze a global Superstore dataset and develop a comprehensive dashboard to track key financial performance metrics, identify regional sales trends, and break down profitability by customer segment and product category.

---

## 🚀 Technologies Used
This project leverages a modern data analysis stack, covering data processing, database management, exploratory analysis, and visualization.

Database Management: PostgreSQL (for table definition in pgAdmin)

Data Analysis & ETL: Python, Pandas, SQLAlchemy

Exploratory Data Analysis (EDA): Google Colab / Jupyter Notebooks

Visualization & Reporting: Microsoft Power BI Desktop

---


## 📁 Project Structure
The repository is organized to ensure all project components (code, data, analysis, and final reports) are easily accessible and reproducible:

sales_dashboard_project/
├── dashboards/                  # Contains the final Power BI file
│   └── Superstore_Sales_Dashboard_Final.pbix
├── data/
│   ├── raw/                     # Original, untouched dataset
│   │   └── Sample - Superstore
│   └── cleaned/                 # Intermediate database file (sales_data)
├── docs/                        # Static reports and exports
│   ├── Superstore_Sales_Dashboard.pdf
│   └── Superstore_Sales_Dashboard_Final_Screenshot.PNG
├── notebooks/                   # Detailed Exploratory Data Analysis (EDA)
│   └── sales_analysis.ipynb
├── sql/                         # Reusable SQL queries
│   ├── create_superstore_table.sql
│   ├── count_orders.sql
│   └── sales_by_region.sql
└── README.md

---

## 📊 Key Dashboard Insights
The Power BI Dashboard () provides a high-level view of business performance, focusing on:

1. High-Level Metrics: Total Sales (2.297K), Total Profit (286K), and Total Orders (9,994).

2. Profitability Breakdown: Detailed visualization of profit across Product Categories (e.g., Technology) and Customer Segments (e.g., Consumer, Corporate, Home Office).

3. Regional Analysis: Ability to filter and drill down into performance by Region (Central, East, South, West).

---


## 🛠️ Data Processing Workflow
The analysis followed these key steps:

1. Database Schema Definition (pgAdmin): The create_superstore_table.sql file defines the schema for the raw data, specifying column types like VARCHAR(50), DATE, and NUMERIC to prepare the PostgreSQL environment for data ingestion.

2. Data Loading (Colab): The sales_analysis.ipynb notebook was used to read the raw CSV data into a Pandas DataFrame and subsequently connect to and load the data into an SQLite database (sales_data.db) using SQLAlchemy.

3. Exploratory Analysis (SQL): Key analytical queries were executed to summarize the data (e.g., sales_by_region.sql).

4. Visualization (Power BI): The cleaned data was connected to Power BI to design the final interactive dashboard.

---


## 💡 How to Run the Project
To view or reproduce the analysis:

1. Clone the Repository: Download the project files locally.

2. View the Dashboard: Open dashboards/Superstore_Sales_Dashboard_Final.pbix in Power BI Desktop.

3. Review the Analysis: Open notebooks/sales_analysis.ipynb in a Jupyter environment (like Google Colab or VS Code) to see the code execution and results.

4. Inspect the SQL: Review the .sql files in the sql/ folder to see the database schema and native queries.