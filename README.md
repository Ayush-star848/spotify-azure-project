# spotify-azure-project
🥉 Bronze Layer – Raw Data Ingestion

The Bronze layer stores raw data exactly as it arrives from the source system.

Key Characteristics

Raw ingestion from Spotify data source

Minimal transformation

Stored in Delta format

Maintains historical records

Example Tables

Raw streaming events

Raw user activity data

Purpose:

Preserve original data

Enable reprocessing if required

🥈 Silver Layer – Data Cleaning & Transformation

The Silver layer processes raw data from Bronze and transforms it into clean, structured datasets.

Transformations Performed

Data cleaning

Schema standardization

Deduplication

Data validation

Creation of dimension and fact tables

Example Tables

DimUser

DimTrack

DimArtist

FactStream

Purpose:

Provide reliable datasets for analytics

Improve data consistency

🥇 Gold Layer – Business Analytics

The Gold layer contains aggregated and business-ready datasets optimized for reporting and analytics.

Example Use Cases

Most streamed artists

Top tracks by listening duration

User engagement metrics

Country-level streaming statistics

Purpose:

Enable dashboards and BI reporting

Provide insights for business decisions

⚙️ Technologies Used
Technology	Purpose
Azure Databricks	Data processing platform
Apache Spark	Distributed data processing
Delta Lake	Reliable data storage
Azure Data Factory	Data orchestration
Jinja	Dynamic SQL generation
GitHub	Version control
