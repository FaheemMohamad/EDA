

# 📊 SQL Data Analytics Project

## 🚀 Overview

This project demonstrates how to perform **end-to-end exploratory data analysis (EDA)** and build **analytical reports** using SQL on a retail-style star schema.
It covers everything from **basic schema exploration** to **advanced trend analysis, customer segmentation, and reporting views**.

The goal is to showcase **SQL analytics skills** for BI, data engineering, and data science use cases.

---

## 🏗️ Database Schema

The project assumes a **data warehouse** with a **star schema** structure:

* **Fact Table**

  * `gold.fact_sales` – transactional sales data

* **Dimension Tables**

  * `gold.dim_customers` – customer attributes
  * `gold.dim_products` – product attributes

---

## 📂 Project Structure

All SQL scripts are located in the `scripts/` folder:

| Category           | Script                       | Purpose                                                     |
| ------------------ | ---------------------------- | ----------------------------------------------------------- |
| 🔎 Exploration     | `database_exploration.sql`   | Explore schema, tables, and columns                         |
| 📅 Date Ranges     | `date_range_exploration.sql` | Find temporal boundaries (first/last orders, customer ages) |
| 📏 Measures        | `measures_exploration.sql`   | Calculate KPIs (sales, orders, customers, products)         |
| 📊 Magnitude       | `magnitude_analysis.sql`     | Aggregate metrics by country, gender, category              |
| 🏆 Ranking         | `ranking_analysis.sql`       | Rank top products/customers by revenue                      |
| 📈 Time Trends     | `change_over_time.sql`       | Monthly/Yearly sales trends                                 |
| 🧮 Cumulative      | `cumulative_analysis.sql`    | Running totals & moving averages                            |
| 📉 Performance     | `performance_analysis.sql`   | Year-over-Year & average benchmarks                         |
| 👥 Segmentation    | `segmentation_analysis.sql`  | Customer & product segmentation                             |
| 🥧 Part-to-Whole   | `part_to_whole_analysis.sql` | % contribution to total sales                               |
| 👤 Customer Report | `customer_report.sql`        | Creates `gold.report_customers` view with KPIs              |
| 📦 Product Report  | `product_report.sql`         | Creates `gold.report_products` view with KPIs               |

---

## 📑 Key Analyses

* **Exploration** → Understand schema, tables, and data ranges
* **KPIs** → Sales, orders, products, customers, revenue
* **Segmentation** → Customer groups (VIP, Regular, New), product cost ranges
* **Trend Analysis** → Time-series (monthly/yearly), running totals, moving averages
* **Ranking** → Top products, top customers, low performers
* **Part-to-Whole** → Contribution of categories to total revenue
* **Reports** → Reusable SQL views for customer & product dashboards

---

## ⚙️ How to Use

1. Clone the repository

   ```bash
   git clone https://github.com/your-username/sql-data-analytics-project.git
   cd sql-data-analytics-project
   ```
2. Run the SQL scripts in your **SQL environment** (e.g., SQL Server, Azure Data Studio, DBeaver).
3. Make sure your database schema matches the expected tables:

   * `gold.fact_sales`
   * `gold.dim_customers`
   * `gold.dim_products`
4. Use the `customer_report.sql` and `product_report.sql` scripts to create reporting views.

---

## 📊 Example Outputs

* **Customer Report View (`gold.report_customers`)**

  * Segmentation (VIP, Regular, New)
  * Recency, Lifespan, Average Order Value
* **Product Report View (`gold.report_products`)**

  * Segmentation (High, Mid, Low performers)
  * Avg Selling Price, Monthly Revenue, Orders & Customers

---

## 🎯 Learning Objectives

* Practice **SQL for analytics & BI**
* Understand **data warehouse exploration**
* Build **customer & product reports** from transactional data
* Apply **window functions, aggregations, segmentation, and ranking**
