# Banking Transactions ETL using Databricks (Medallion Architecture)

## Project Overview
This project implements a Medallion Architecture (Bronze, Silver, Gold) ETL pipeline using Databricks and PySpark on banking transaction data.

## Data Sources
- bank_data.csv
- customer_data.csv
- transaction_data.csv

## Architecture

### Bronze Layer
Raw CSV files ingested into Delta tables.

### Silver Layer
- Joined customer and transaction data
- Data cleaning and transformations
- Fraud flag logic
- Derived year and month columns

### Gold Layer
Customer monthly spending aggregation for business analytics.

## Technologies Used
- Databricks
- PySpark
- Delta Lake
- Unity Catalog

## Tables Created
- bronze_bank
- bronze_customer
- bronze_transaction
- silver_transactions
- gold_customer_monthly
