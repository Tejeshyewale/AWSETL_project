# AWSETL_project Theory of Services used 
Build a serverless ETL pipeline using AWS Glue to process and analyze CSV data stored in S3 with Athena.
1. AWS S3 (Simple Storage Service)
•	What is it? 
o	Object storage service that provides scalable, secure, and high-performance storage.
•	Key Features: 
o	Stores data as objects in buckets.
o	Highly available, durable, and cost-effective.
o	Supports multiple storage classes (Standard, IA, Glacier, etc.).
o	Queryable with Athena (without moving data).
o	Integrated with AWS Glue for ETL processes.
•	Use Cases: 
o	Data lake storage.
o	Backup and archival.
o	Hosting static websites.
________________________________________
2. AWS Glue
•	What is it? 
o	A fully managed ETL (Extract, Transform, Load) service that prepares data for analytics.
•	Key Components: 
o	Glue Crawler: Automatically scans S3 and creates metadata in the Glue Data Catalog.
o	Glue Data Catalog: Stores metadata for structured/semi-structured data.
o	Glue Jobs: Runs transformations using PySpark or Python shell scripts.
•	Key Features: 
o	Serverless (scales automatically).
o	Supports schema inference.
o	Can integrate with Athena, Redshift, and RDS.
o	Supports partitioning and cataloging for better performance.
•	Use Cases: 
o	Cleaning and transforming raw data from S3.
o	Automating data pipelines for machine learning.
o	Migrating and preparing data for analytics.
________________________________________
3. AWS Athena
•	What is it? 
o	A serverless query service to analyze data directly from S3 using SQL.
•	Key Features: 
o	Uses Presto (open-source SQL engine).
o	Queries data without loading it into a database.
o	Supports structured and semi-structured formats (CSV, JSON, Parquet, ORC).
o	Works with Glue Data Catalog for metadata management.
o	Pay-per-query pricing model (cost-efficient).
•	Use Cases: 
o	Ad-hoc querying of large datasets in S3.
o	Log analysis and reporting.
o	Business intelligence and analytics.
________________________________________
How They Work Together
1.	Store raw data in S3 → (data lake storage).
2.	Use AWS Glue Crawler → (automatically infer schema & create metadata in Glue Data Catalog).
3.	Run AWS Glue Jobs → (clean and transform data if needed).
4.	Query data using Athena → (run SQL queries directly on S3 without moving data).
This combination is widely used for big data analytics and serverless data pipelines. 🚀

