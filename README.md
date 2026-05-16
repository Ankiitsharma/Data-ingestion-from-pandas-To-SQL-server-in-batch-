File 1: Data Ingestion Pipeline
Purpose

This script:

Connects to MySQL database
Creates employee_data table
Reads employee CSV data
Inserts records into MySQL in batches
Maintains pipeline logs

CSV File
   ↓
Pandas DataFrame
   ↓
SQLAlchemy Connection
   ↓
MySQL Table (employee_data)

Features
Batch insertion
Logging support
Exception handling
Table creation using SQLAlchemy
CSV ingestion


File 2: Data Transformation Pipeline
Purpose

This script:

Reads data from MySQL
Converts Pandas DataFrame to Spark DataFrame
Performs basic PySpark transformations
Checks NULL values
Writes transformed data back to MySQL

MySQL Table
   ↓
Pandas DataFrame
   ↓
Spark DataFrame
   ↓
PySpark Transformations
   ↓
Pandas DataFrame
   ↓
MySQL Target Table

Features
Pandas to Spark conversion
NULL validation
Spark transformations
Writing transformed data to MySQL

Author

Ankit Sharma
Data Engineering | PySpark | SQL | Databricks
