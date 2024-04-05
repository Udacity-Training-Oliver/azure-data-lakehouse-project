# Azure Data Lakehouse Project

## Delta Lake Architecture

- **Bronze Layer**: This is the raw data ingestion layer where data is stored in its raw, unprocessed form. No schema or data type enforcement is typically done at this layer.
- **Silver Layer**: This is the cleaned and processed data layer. At this stage, data is transformed from its raw form into a structured form, which involves defining the data types for each column. This layer is typically used for exploratory data analysis and to create derived datasets.
- **Gold Layer**: This layer contains business-level aggregates, often used for reporting and dashboarding. The schema for this layer is typically derived from the silver layer. As such, while some additional transformation and aggregation may occur in this layer, the underlying data types are usually already defined in the silver layer.


![Star Schema](./images/star_schema.png)

![Databricks Cluster Configuration](./images/cluster_configuration.png)

![DBFS Raw Data](./images/dbfs_raw_data.png)

![DBFS Bronze Delta](./images/dbfs_bronze_delta.png)

![Metastoe Silver Gold](./images/metastore_silver_gold.png)

![Jupyter Notebooks](./images/notebooks.png)
