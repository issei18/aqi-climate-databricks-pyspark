# Climate AQI Databricks PySpark Pipeline

End-to-end Bronze → Silver → Gold data engineering pipeline built using Databricks, PySpark, and AWS S3 to process and analyze Air Quality Index (AQI) and climate data.

## Tech Stack
- Databricks
- PySpark
- AWS S3
- Parquet
- Spark SQL

## Architecture (Medallion Pattern)
Raw Data (CSV)
→ Bronze Layer: Raw ingestion, partitioned by year/month  
→ Silver Layer: Cleaned, standardized, and type-casted data  
→ Gold Layer: Aggregated metrics and AQI rankings  

## Key Features
- Bronze–Silver–Gold ETL design
- Column standardization and data type casting
- Year and month partitioning for optimized storage
- Spark Window functions for pollution ranking
- Parquet-based curated datasets
- Cloud-ready S3 data lake structure

## Gold Layer Output
- City-wise monthly average AQI
- Pollution ranking by year and month
- Partitioned Parquet files for analytics and reporting

## Repository Structure
AQI_databricks_pipeline.ipynb  # Complete end-to-end ETL pipeline
README.md

## Use Case
This project demonstrates real-world data engineering practices including scalable ETL pipelines, data lake layering, performance-aware partitioning, and analytical transformations using PySpark.

## Author
Vedang Kharsamble  
Data Engineering | PySpark | Databricks | AWS
