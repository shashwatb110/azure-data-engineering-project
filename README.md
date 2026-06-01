# Azure Data Engineering Project

## Overview

This project demonstrates an end-to-end Azure Data Engineering pipeline built using Azure services and Databricks. The solution focuses on ingesting, transforming, and processing data using scalable cloud-based technologies following modern data engineering practices.

The project showcases data ingestion, transformation, storage, and analytics workflows commonly used in enterprise environments.

---

## Architecture

![Architecture Diagram](<img width="1037" height="622" alt="image" src="https://github.com/user-attachments/assets/35451b96-6081-4f5d-a4c7-965d13188b11" />)

### Data Flow

1. Data is ingested from the source system.
2. Raw data is stored in the Bronze layer.
3. Data transformation and cleansing are performed using Azure Databricks and PySpark.
4. Processed data is stored in the Silver layer.
5. Business-ready data is loaded into the Gold layer.
6. Data can be consumed for reporting and analytics.

---

## Technologies Used

- Azure Databricks
- PySpark
- Delta Lake
- Azure Data Lake Storage Gen2 (ADLS)
- Azure Data Factory (ADF)
- Azure Synapse Analytics
- SQL
- Power BI

---

## Project Structure

```text
azure-data-engineering-project/
│
├── notebooks/
│   ├── data_ingestion
│   ├── data_transformation
│   └── data_loading
│
├── datasets/
│
├── screenshots/
│
├── architecture/
│
└── README.md
```

## Key Features

- End-to-End Data Pipeline
- Data Ingestion using Azure Services
- Data Transformation with PySpark
- Delta Lake Implementation
- Incremental Data Processing
- Scalable Cloud Architecture
- Data Quality Validation
- Medallion Architecture (Bronze, Silver, Gold)

---

## Databricks Transformations

Some of the transformations implemented include:

- Data cleansing
- Null handling
- Column standardization
- Data type conversion
- Deduplication
- Aggregations
- Delta Table operations
- Merge and Upsert operations

---

## Sample PySpark Operations

```python
from delta.tables import DeltaTable
from pyspark.sql import functions as F

df = (
    df
    .withColumn("created_timestamp", F.current_timestamp())
    .withColumn("updated_timestamp", F.current_timestamp())
)
```

---

## Business Use Case

The objective of this project is to build a scalable and reliable cloud data platform capable of processing large datasets and preparing them for analytics and reporting.

This architecture can be applied to:

- Retail Analytics
- Sales Reporting
- Customer Insights
- Financial Analytics
- Operational Dashboards

---

## Screenshots
<img width="1493" height="812" alt="image" src="https://github.com/user-attachments/assets/b172564d-09e2-4c80-84b2-00b47f68971a" />
<img width="1496" height="815" alt="image" src="https://github.com/user-attachments/assets/8f535cde-f31b-447c-9b48-0e00847f293f" />
<img width="1486" height="753" alt="image" src="https://github.com/user-attachments/assets/14c57284-70e8-461e-9d16-e10961106aa2" />
<img width="1515" height="783" alt="image" src="https://github.com/user-attachments/assets/b8181ad0-8e18-4069-a285-9a25c249977b" />
<img width="1383" height="393" alt="image" src="https://github.com/user-attachments/assets/904ab229-4064-463b-b635-06393fcfe11a" />



### Azure Databricks

Add screenshots of:
- Notebooks
- Cluster Configuration
- Workflow Jobs

### Azure Data Factory

Add screenshots of:
- Pipelines
- Copy Activities
- Trigger Runs

### Data Lake Storage

Add screenshots of:
- Bronze Layer
- Silver Layer
- Gold Layer

---

## Future Enhancements

- CI/CD Integration
- GitHub Actions Deployment
- Automated Monitoring
- Data Quality Framework
- Unity Catalog Integration
- Real-Time Streaming Pipelines

---

## Author

Shashwat Bhardwaj

GitHub:
https://github.com/shashwatb110

LinkedIn:
https://www.linkedin.com/in/shashwat-bhardwaj-15a25a24b/?skipRedirect=true

---

## Project Status

Completed and actively maintained.
