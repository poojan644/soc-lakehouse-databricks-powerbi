## Databricks Notebooks

This folder contains Databricks notebooks used to build the SOC Lakehouse pipeline.

### Notebooks Included
- **01_soc_ingest_raw_to_silver**
  - Ingests raw security logs from ADLS Gen2
  - Cleans, normalizes, and enriches data
  - Writes Delta tables to the Silver layer

- **02_soc_silver_to_gold**
  - Aggregates security events
  - Creates analytical datasets (failed logins, critical events, trends)
  - Writes Delta tables to the Gold layer

### Technologies Used
- Azure Databricks
- PySpark
- Delta Lake
- Azure Data Lake Storage Gen2

