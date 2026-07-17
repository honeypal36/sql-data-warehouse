# SQL Data Warehouse Project

A modern Data Warehouse implementation built using SQL that demonstrates the complete data engineering workflow-from raw data ingestion to business-ready analytical models.

## 📌 Project Overview

This project implements a layered Data Warehouse architecture to transform raw operational data into clean, structured, and analytics-ready datasets.

The project covers:

- Data Warehouse design
- ETL (Extract, Transform, Load) pipeline
- Data cleaning and transformation
- Data modeling
- Business-ready analytical views
- SQL-based reporting

---

## 🏗️ Architecture

The warehouse follows a **Medallion Architecture** consisting of three layers:

```
           Source Systems
                 │
                 ▼
        🥉 Bronze Layer
     (Raw Source Data)
                 │
                 ▼
        🥈 Silver Layer
 (Cleaned & Standardized Data)
                 │
                 ▼
         🥇 Gold Layer
(Business Ready Data Model)
```

### Bronze Layer
- Stores raw source data
- Minimal transformations
- Maintains historical records

### Silver Layer
- Cleans and validates data
- Removes duplicates
- Standardizes formats
- Handles missing values

### Gold Layer
- Business-ready tables
- Fact and Dimension modeling
- Optimized for reporting and analytics

---

## 📂 Project Structure

```
sql-data-warehouse/
│
├── datasets/
│   ├── source_crm/
│   └── source_erp/
│
├── scripts/
│   ├── bronze/
│   ├── silver/
│   ├── gold/
│   └── init_database.sql
│
├── docs/
│
└── README.md
```

---

## ⚙️ Technologies Used

- SQL
- SQL Server
- ETL
- Data Warehousing
- Star Schema
- Data Modeling

---

## 🔄 ETL Workflow

1. Load raw CRM and ERP datasets
2. Store data in Bronze layer
3. Clean and transform data into Silver layer
4. Build analytical models in Gold layer
5. Execute SQL queries for business insights

---

## ⭐ Data Modeling

The Gold layer follows a **Star Schema** consisting of:

### Fact Tables
- Sales Fact

### Dimension Tables
- Customers
- Products
- Date
- Category
- Geography

---

## 📊 Business Insights

This warehouse can be used to answer business questions such as:

- Total Sales
- Monthly Revenue Trends
- Best Selling Products
- Customer Segmentation
- Product Performance
- Regional Sales Analysis
- Top Customers
- Sales by Category

---

## 🚀 Getting Started

### Clone Repository

```bash
git clone https://github.com/honeypal36/sql-data-warehouse.git
```

### Open SQL Server

Run the scripts in the following order:

```
1. init_database.sql
2. Bronze Layer Scripts
3. Silver Layer Scripts
4. Gold Layer Scripts
```

Finally, execute the analytical SQL queries.

---

## 🎯 Learning Outcomes

Through this project, I learned:

- Data Warehouse Architecture
- ETL Pipeline Development
- SQL Optimization
- Data Cleaning
- Star Schema Design
- Fact & Dimension Modeling
- Business Analytics using SQL

---

## 📈 Future Improvements

- Power BI Dashboard
- Automated ETL Scheduling
- Incremental Data Loading
- Data Quality Checks
- Performance Optimization
- Stored Procedures & Indexing

---

## 👨‍💻 Author

**Honey Pal**

- GitHub: https://github.com/honeypal36
- LinkedIn: https://www.linkedin.com/in/honey-pal-520983335

---

## ⭐ If you found this project useful, consider giving it a star!
