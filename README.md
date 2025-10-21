# Snowpipe Auto-Ingest Pipeline from GCS to Snowflake

## 🚀 Project Overview

This project demonstrates how to set up **Snowpipe** to automatically ingest data from **Google Cloud Storage (GCS)** into a **Snowflake table**. Snowpipe allows **continuous data ingestion** in near real-time using **Pub/Sub notifications**.

The pipeline includes:

- Snowflake Database and Table creation
- GCS Storage Integration
- Stage creation for file landing
- Pub/Sub notification integration
- Auto-ingest Snowpipe configuration
- Monitoring and troubleshooting

---

## 📁 Prerequisites

- A **Snowflake account** with `ACCOUNTADMIN` or appropriate roles.
- A **Google Cloud Platform (GCP) project** with a GCS bucket containing CSV files.
- Pub/Sub enabled in your GCP project.
- Proper IAM permissions to create service accounts and assign roles for Snowflake integration.


```sql
-- Use the account admin role
USE ROLE accountadmin;

-- Create database for Snowpipe development
CREATE OR REPLACE DATABASE snowpipe_dev;
