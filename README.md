Snowflake S3 ETL & BI Insights

This project implements a data pipeline to extract, clean, and load customer, transaction, and date data from S3 into Snowflake. The pipeline standardizes column names and formats, ensures idempotency, and performs aggregations for fiscal weekly, monthly, and quarterly metrics.

Key Highlights:

ETL Pipeline: Reads CSV files from S3, cleans and standardizes data, deduplicates rows, and loads them into Snowflake tables. Automatically creates or updates tables as needed.

Data Standardization: Aligns transaction dates with fiscal calendar, maps column variants, and ensures consistent formats for analysis.

Business Insights: Computes sales, refunds, net revenue, and total items. Segments customers by value, identifies top spenders and most frequent buyers.

Refunds: Calculates final refund amounts after a 10% restocking fee.

Visualization: Interactive dashboards in Jupyter notebooks with tables and charts for top customers and financial metrics.

Idempotency: Re-running scripts will not duplicate data, preserving data integrity.

Security: Uses Snowflake access credentials and AWS IAM role for secure S3 access.

Purpose:
Provides a framework to generate daily insights, monitor top customers, and support financial and operational decision-making.
