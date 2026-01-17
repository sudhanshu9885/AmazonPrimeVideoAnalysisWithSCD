# Amazon Prime Movies & TV Shows Analytics Pipeline  
**Databricks Medallion Architecture for Scalable Streaming Content Analytics**  

**Build a robust pipeline to analyze Amazon Prime content, providing actionable insights on trends, ratings, and audience targeting.**  

---

## Tools & Technologies
- **Data Platform:** Azure Databricks, Databricks Volumes, Delta Lake  
- **Processing Engine:** Apache Spark  
- **Dataset:** Kaggle Amazon Prime Movies & TV Shows Dataset  

---

## Key Features

- **Data Ingestion (Bronze Layer):**  
  Ingested raw Amazon Prime Movies & TV Shows data directly from backend storage into Databricks Volumes, preserving original schema and format for full data lineage and traceability.

- **Data Cleaning & Transformation (Silver Layer):**  
  Processed Bronze-layer data using Databricks notebooks and Spark to enforce schema consistency, remove duplicates, handle null values, and cast data types.  
  Applied feature engineering: extracted duration in minutes, created adult-content flags, and split datasets into `movies_silver` and `tv_shows_silver` for targeted analysis.

- **Data Modeling & Optimization:**  
  Stored curated datasets in Delta format for ACID compliance, incremental processing, and enhanced query performance. Leveraged Delta Lake features for reliability and scalability.

- **Analytical Layer (Gold Layer):**  
  Built Gold-layer Delta tables and views for business-ready insights: content distribution by type, top-duration titles, rating statistics, country-wise breakdowns, and release trends over time.

- **Pipeline Architecture:**  
  Designed a full end-to-end Databricks pipeline following Bronze–Silver–Gold medallion architecture, enabling structured data processing, scalability, and maintainability.

---

## Business Impact
Delivered efficient large-scale content analytics, supporting advanced analytics, BI integrations, and actionable insights for catalog optimization, audience targeting, and data-driven content strategies.

