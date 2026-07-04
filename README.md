# olist-ecommerce-databricks-pipeline
This repository contains the architecture and codebase for an end-to-end E-commerce Analytics pipeline built on the Databricks Data Intelligence Platform. Utilizing the Olist Brazilian E-commerce dataset, the project demonstrates a complete "Medallion Architecture" workflow.

# Olist E-commerce Data Pipeline on Databricks

## Project Overview
This project implements a scalable data engineering pipeline and BI solution for e-commerce data using **Databricks** and **Delta Lake**. It transforms raw transactional data into a curated "Gold" layer for executive reporting.

## Tech Stack
- **Platform:** Databricks (Cloud Edition)
- **Storage:** Delta Lake (Medallion Architecture)
- **Language:** Spark SQL, Python (Databricks SDK)
- **Orchestration:** Databricks Jobs & Workflows
- **Visualization:** Databricks AI-BI Dashboards
- **AI Integration:** Databricks Genie (Natural Language to SQL)

## Pipeline Architecture
1. **Raw Layer:** Ingestion of Olist datasets (orders, customers, payments, products).
2. **Silver Layer:** Joined tables (e.g., `silver_sales`) providing a unified view of transactions and items.
3. **Gold Layer:** Aggregated tables (e.g., `gold_category_performance`) optimized for dashboarding.

## Key Insights & Features
- **Automated Workflows:** Scheduled jobs to ensure data freshness.
- **Revenue Analytics:** Tracking of monthly trends and top-performing product categories.
- **Payment Analysis:** Breakdown of revenue by payment type (Credit Card, Boleto, etc.).
- **Natural Language Querying:** Use of Genie Spaces to allow ad-hoc data questions.

## How to Use
- Import the `.ipynb` notebook into your Databricks workspace.
- Use the `databricks_job_config.py` to recreate the automated workflow via the Databricks SDK.
- Import `ecommerce_dashboard.json` in the SQL/Dashboards tab to view visualizations.
