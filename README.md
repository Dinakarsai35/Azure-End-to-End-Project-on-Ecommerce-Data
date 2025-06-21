## 🛒 Azure Data Engineering Project – eCommerce Dataset

## 🚀 End-to-End Azure Data Engineering Project using Medallion Architecture and eCommerce Sales Data

This project simulates a real-time enterprise-grade Azure data pipeline by ingesting, transforming, and modeling eCommerce sales data using a lakehouse approach. The solution leverages GitHub, ADF, Azure SQL, Azure Data Lake, Azure Databricks, and Power BI — following best practices and automation.

## 📌 Project Architecture Overview


Bronze → Silver → Gold Medallion Architecture

GitHub → Azure Data Factory → Azure SQL Database → Azure Data Lake → Azure Databricks → Power BI

## 🔧 Tools & Services Used
GitHub – Hosted raw CSV files and incremental dataset

Azure Data Factory (ADF) – Used for initial and incremental ingestion with Lookup, ForEach, and Copy Activity

Azure SQL Database – Staging layer for data validation and type adjustment

Azure Data Lake Storage Gen2 – Used for storing raw (Bronze), cleansed (Silver), and business-ready (Gold) data

Azure Databricks (with Unity Catalog) – Transformation engine using PySpark; schema enforcement and lineage

Power BI – Final reporting layer connected to Gold data

Stored Procedures – For tracking last loaded data

Unity Catalog – Data governance and access control in Databricks

## 🔑 Key Highlights

✅ Ingested data from GitHub to Azure SQL with type casting

✅ Created stored procedures for incremental tracking

✅ Built Medallion architecture: Bronze → Silver → Gold

✅ Enabled Unity Catalog in Databricks

✅ Built Star & Snowflake Schema in Gold Layer

✅ Attached Databricks notebooks to ADF for end-to-end automation

✅ Visualized Gold data in Power BI dashboard

## 🧱 Implementation Summary
 Data Loading

Uploaded dataset to GitHub using git commands

Included incremental dataset for simulation

Created Copy activity in ADF to ingest from GitHub to Azure SQL

Performed data type adjustments in SQL

Created Stored Procedure to track last loaded record

Bronze Layer – Raw Storage

Moved validated data from Azure SQL to ADLS Bronze folder via ADF

Incremental Load

Configured Lookup for last and current load in ADF

Handled incremental ingestion logic

Silver & Gold Layer – Transformations

Enabled Unity Catalog in Databricks

Built Databricks notebooks for cleansing and enrichment

Transformed and loaded Silver and Gold layer data to ADLS

Modeled Star & Snowflake schemas in Gold

Automation & Visualization

Scheduled Databricks notebook from ADF

Connected Power BI to Gold layer

Created business dashboards for reporting



## 📊 Final Output
An automated, scalable Azure data pipeline with proper data governance, schema modeling, and Power BI reporting using real-world eCommerce data.

## 🙏 Credits
This project was inspired by the YouTube tutorial by Ansh Lamba:

🔗 [Watch here](https://www.youtube.com/watch?v=6_hXeNg9TJ0)

## 👨‍💻 Author
Dinakar Sai Gullapalli

📧 sai4.gullapalli@gmail.com

🔗 [GitHub Project](https://github.com/Dinakarsai35/Azure-End-to-End-Project-on-Ecommerce-Data)  


🔗 [LinkedIn Profile](https://www.linkedin.com/in/dinakar-sai-gullapalli-52469915b/)
