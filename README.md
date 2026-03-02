# Azure Databricks ETL Pipeline (DLT-Based Lakehouse)

This project implements an end-to-end **ETL pipeline using Azure Databricks** with a **lakehouse architecture**. It supports **dynamic data ingestion**, **incremental loading**, **slowly changing dimensions (SCD)**, and **star schema modeling**, leveraging **Delta Live Tables (DLT)** for reliable and scalable data processing.

---

## 📌 Project Overview

The pipeline is designed to process data from multiple source systems dynamically and transform it into analytics-ready datasets. It follows modern data engineering best practices, including incremental processing, dimensional modeling, and declarative pipeline orchestration using Delta Live Tables.

---

## ✨ Key Features

- **Dynamic Data Ingestion**
  - Metadata-driven ingestion framework
  - Supports multiple source tables without code duplication

- **Incremental Loading**
  - Processes only new or changed data
  - Improves performance and reduces compute cost

- **Slowly Changing Dimensions (SCD)**
  - Implements SCD Type 1 and Type 2
  - Maintains historical data changes where required

- **Star Schema Design**
  - Fact and dimension tables modeled for analytics
  - Optimized for BI and reporting workloads

- **Delta Live Tables (DLT)**
  - Declarative pipeline definitions
  - Built-in data quality checks and dependencies
  - Automated table management and monitoring

---

## 🏗️ Architecture

The pipeline follows the **Medallion Architecture**:

- **Bronze Layer**
  - Raw ingested data
  - Incremental ingestion from source systems

- **Silver Layer**
  - Cleaned and transformed data
  - Business logic applied
  - SCD handling implemented

- **Gold Layer**
  - Star schema (fact and dimension tables)
  - Aggregated, analytics-ready datasets

---


---

## ⚙️ Technologies Used

- Azure Databricks
- Apache Spark (PySpark)
- Delta Lake
- Delta Live Tables (DLT)
- Azure Data Lake Storage (ADLS Gen2)
- GitHub (Version Control)

---

## 🚀 Pipeline Execution

The pipeline can be executed using **Delta Live Tables**:

1. Clone the repository into **Databricks Repos**
2. Configure secrets using **Databricks Secret Scopes**
3. Update metadata and environment settings in `configs/config.yaml`
4. Create and run a **DLT Pipeline** using the scripts under the `dlt/` directory

---

## 🔐 Secrets & Configuration

- No credentials are hardcoded
- Secrets are managed using Databricks Secret Scopes
- Environment-specific values are externalized via configuration files

---

## 📈 Future Enhancements

- Integrate BI tools for reporting
- Implement CI/CD using GitHub Actions
- Add automated unit and integration tests

---


**Ramreddy Arolla**  
Graduate Student | Arizona State University 
