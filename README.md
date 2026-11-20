# Customer Data Processing Pipeline

## Project Overview
An end-to-end Data Engineering project developed using Azure Databricks and PySpark.

## Technologies Used
- Azure Databricks
- PySpark
- Delta Lake
- Unity Catalog
- Databricks Workflows
- SQL

## Architecture

CSV Source → Bronze → Silver → Gold → Data Validation

## Pipeline Implementation

### 1. Bronze Layer
- Ingested raw customer CSV data.
- Stored data as a Delta table.

### 2. Silver Layer
- Removed duplicate customer records.
- Handled NULL values.
- Trimmed customer names.
- Validated email addresses.
- Separated valid and rejected records.

### 3. Gold Layer
- Calculated total customers.
- Generated city-wise customer counts.
- Calculated average salary by city.
- Identified high-salary customers.

### 4. Data Validation
- Checked duplicate records.
- Checked NULL values.
- Validated email addresses.
- Verified record counts.

## Workflow Orchestration

Created a Databricks Workflow with four dependent notebook tasks:

1. Bronze Ingestion
2. Silver Transformation
3. Gold Transformation
4. Data Validation

All four tasks executed successfully.

## Project Outcome
Successfully developed and executed an end-to-end customer data processing pipeline using Databricks and PySpark.
