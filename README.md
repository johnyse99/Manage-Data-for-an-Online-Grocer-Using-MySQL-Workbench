# Greenspot Grocer - Relational Database Design

## Project Overview

Greenspot Grocer is a rapidly growing family-owned online grocery store. This project involves transitioning their inventory and sales data from a flat-file spreadsheet format to a robust, scalable **MySQL Relational Database**.

The goal is to eliminate data redundancy, ensure data integrity through normalization (3NF), and provide a foundation for business expansion.

## Key Features

- **3NF Normalization**: Minimized data redundancy by separating Vendors, Products, Units, and Categories into dedicated tables.
- **Storage Optimization**: Strategic use of data types (`TINYINT`, `SMALLINT`, `UNSIGNED`) to reduce disk space and improve query performance.
- **Relational Integrity**: Implementation of Primary Keys and Foreign Keys to prevent orphan records.
- **Business Intelligence**: Advanced SQL JOIN queries to track inventory levels, sales history, and profitability.

## Repository Structure

- `data/`: Contains the original source dataset (`.csv`).
- `reports/`: Documentation on database design, anomalies analysis, and normalization steps.
- `sql_scripts/`:
  - `create_database.sql`: Schema definition (DDL).
  - `load_data.sql`: Data population script (DML).
  - `verify_queries.sql`: Initial verification tests.
  - `check_relationships.sql`: Relationship validation.
  - `insert_new_product.sql`: Example of maintaining referential integrity during insertions.
  - `business_report_query.sql`: Complex query for profitability analysis.

## Getting Started

1. Clone this repository.
2. Open **MySQL Workbench**.
3. Execute the scripts in the following order:
   1. `sql_scripts/create_database.sql`
   2. `sql_scripts/load_data.sql`
4. Use the remaining scripts in `sql_scripts/` to verify and test the database functionality.

## Business Insights

The database allows the owner to answer critical questions such as:

- Which products are low on stock and who is the preferred vendor?
- What is the total profit generated per sale after calculating purchase costs?
- Which categories are performing best in terms of sales volume?

## Author

_Project developed as part of the Coursera Data Analysis Professional Certificate._
