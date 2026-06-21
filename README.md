# 🏢 SQL Data Warehouse Project

## 📌 Project Overview

This project demonstrates the implementation of a modern **Data Warehouse Solution** using **SQL Server** and **Medallion Architecture**. The project covers data ingestion, ETL processing, data transformation, dimensional modeling, and analytical reporting.

The Medallion Architecture organizes data into multiple layers to improve data quality, maintainability, and analytical performance.

---

## 🏗️ Architecture: Medallion Architecture

The project follows a three-layer Medallion Architecture:

```text
Source Systems
      │
      ▼
┌─────────────────┐
│ Bronze Layer    │
│ (Raw Data)      │
└─────────────────┘
      │
      ▼
┌─────────────────┐
│ Silver Layer    │
│ (Cleaned Data)  │
└─────────────────┘
      │
      ▼
┌─────────────────┐
│ Gold Layer      │
│ (Business Data) │
└─────────────────┘
      │
      ▼
Analytics & Reporting
```

### 🥉 Bronze Layer

* Stores raw data from source systems.
* No business transformations.
* Historical data preservation.
* Serves as the system of record.

### 🥈 Silver Layer

* Data cleansing and standardization.
* Duplicate removal.
* Data quality checks.
* Business rule implementation.

### 🥇 Gold Layer

* Business-ready analytical data.
* Fact and Dimension tables.
* Star Schema implementation.
* Optimized for reporting and dashboards.

---

## 📂 Project Structure

```text
SQL-Data-Warehouse-Project/
│
├── datasets/
│
├── bronze/
│   ├── load_bronze.sql
│   └── bronze_tables.sql
│
├── silver/
│   ├── clean_data.sql
│   ├── transform_data.sql
│   └── silver_tables.sql
│
├── gold/
│   ├── dim_customer.sql
│   ├── dim_product.sql
│   ├── fact_sales.sql
│   └── analytical_views.sql
│
├── diagrams/
│   ├── medallion_architecture.png
│   └── star_schema.png
│
└── README.md
```

---

## ⭐ Key Features

* Modern Medallion Architecture
* SQL Server Data Warehouse
* ETL Pipeline Development
* Bronze, Silver, and Gold Layers
* Star Schema Data Modeling
* Fact and Dimension Tables
* Analytical SQL Queries
* Business Intelligence Ready

---

## 📚 Skills Demonstrated

* SQL Server
* Data Warehousing
* ETL Development
* Data Engineering
* Medallion Architecture
* Dimensional Modeling
* Star Schema Design
* Data Analytics
* Business Intelligence

