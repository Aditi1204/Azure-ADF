# Azure Data Factory Repository
# Airline Analytics Data Pipeline using Medallion Architecture

This project implements an end-to-end data engineering solution using Azure Data Factory, Azure SQL Database, and Azure Data Lake Storage Gen2 following the Medallion Architecture (Bronze, Silver, and Gold layers).

### Architecture

**Bronze Layer**

* Ingested raw booking data from Azure SQL Database into ADLS Gen2.
* Implemented incremental loading using watermark-based processing.
* Stored raw datasets for auditability and historical tracking.

**Silver Layer**

* Performed data cleansing, validation, and standardization.
* Applied transformations using Azure Data Factory Mapping Data Flows.
* Integrated FactBookings with dimension tables (DimAirline, DimFlight, DimPassenger).

**Gold Layer**

* Built business-ready datasets for analytics and reporting.
* Aggregated booking metrics by airline.
* Applied ranking logic to identify the Top 5 performing airlines.
* Delivered curated datasets for Power BI dashboards and business consumption.

### Key Features

* Incremental data loading using watermark JSON files.
* Fact and Dimension data modeling (Star Schema).
* Join, Aggregate, Rank, Filter, and Sink transformations.
* Automated orchestration using Azure Data Factory pipelines.
* Data Lake organization using Bronze, Silver, and Gold layers.

### Technologies

* Azure Data Factory (ADF)
* Azure SQL Database
* Azure Data Lake Storage Gen2 (ADLS)
* Azure Synapse Analytics / Data Warehouse
* Mapping Data Flows
* SQL
* Medallion Architecture
* Dimensional Modeling

### Business Outcome

Provides trusted, business-ready airline performance insights by transforming raw booking data into curated analytical datasets, enabling efficient reporting and decision-making.
