An enterprise, metadata-driven Azure data engineering solution designed to ingest transactional SQL data and deliver scalable analytics via the Medallion Architecture (Bronze, Silver, Gold).

Key Components & Workflow
Ingestion Mechanisms: Implements three distinct ingest strategies depending on business needs:

Full Load, Incremental Load, CDC Load: Captures INSERT, UPDATE, and DELETE operations via SQL Server Change Data Capture.

Orchestration & Storage: Azure Data Factory (ADF) manages pipeline execution and data movement into Azure Data Lake Storage Gen2 (ADLS Gen2).

Transformation & Processing: Azure Databricks processes raw data across Delta Lake layers:

Bronze: Raw data landing zone / Silver: Cleaned, standardized, and normalized data / Gold: Consolidates data into current-state datasets and business-oriented dimensional models (Fact and Dimension tables).

## Architecture

The overall architecture follows a layered modern data engineering pattern:

