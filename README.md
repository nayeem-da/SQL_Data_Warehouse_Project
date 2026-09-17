# SQL-DATAWARHOUSE-PROJECT
Sales Analytics Data Pipeline | SQL Server | Medallion Architecture

This project implements a complete data engineering pipeline using SQL Server following the Medallion Architecture (Bronze → Silver → Gold). The objective is to transform raw CSV data into structured, business -ready analytical models for real-world reporting needs.

Data Sources

Total: 6 CSV files

Customer Data: 2 files with customer details and ID mapping

Product Data: 2 files with product information and ID mapping

Sales Data: 2 files containing transactional sales data linked by Customer ID and Product ID

The combined files form a relational dataset.

Medallion Architecture Workflow

Bronze Layer – Raw Data

CSV files loaded directly into SQL Server

No cleaning or transformations

Acts as the staging layer

Silver Layer – Cleaned and Standardized Data

Data quality checks and missing value handling

Data type formatting and standardization

Lookup joins for enrichment

Derived and normalized fields to support analytics

Gold Layer – Business-Ready Data Model

Designed using Star Schema approach

Fact Table: FactSales

Dimension Tables: DimCustomer, DimProduct

Implemented through SQL Views for optimized querying

SQL Exploratory Data Analysis (EDA)

SQL was used to analyze and validate the data before modeling:

Sales performance by customers and products

Time-based revenue trends

Data distribution and outlier checks

Segmentation insights for analytics use cases

Project Highlights

This project demonstrates:

End-to-end data transformation using SQL Server

Practical implementation of Medallion Architecture

Dimensional modeling for analytics

Clean and efficient data structures suitable for dashboards and reports

Fully documented SQL scripts for repeatable workflows

Technology Stack

SQL Server

T-SQL

CSV files as raw input sources
