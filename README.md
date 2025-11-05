Customer Data ETL Pipeline with PySpark
Project Overview

This project demonstrates a batch ETL (Extract, Transform, Load) pipeline using PySpark. The pipeline processes a customer dataset, performing data cleaning, transformation, and aggregation to produce actionable insights. It is designed to run on distributed systems with HDFS or local storage, illustrating core data engineering concepts such as RDDs, DataFrames, and Spark SQL.

Dataset

The dataset contains customer information with the following fields:

customer_id : Unique identifier for each customer

name : Customer name

city : City of the customer

state : State of the customer

country : Country of the customer

registration_date : Date the customer registered

is_active : Boolean indicating whether the customer is currently active

Sample dataset:

customer_id	name	city	state	country	registration_date	is_active
0	Customer_0	Pune	Maharashtra	India	1/19/2023	TRUE
1	Customer_1	Pune	West Bengal	India	8/10/2023	TRUE
Project Tasks

Data Ingestion

Load raw CSV data into PySpark as RDDs or DataFrames.

Inspect the data to understand column types and quality.

Data Cleaning

Handle missing or null values.

Convert registration_date to a date type.

Convert is_active to boolean.

Remove duplicate records.

Data Transformation

Derive new columns (e.g., year and month of registration).

Filter data based on conditions (e.g., only active customers).

Aggregation & Analytics

Count customers per city, state, or country.

Analyze active versus inactive customers.

Compute monthly registrations to observe trends.

Data Export

Write processed data to HDFS or local storage in CSV or Parquet format.

Optional partitioning for scalable storage.

Optional Enhancements

Cache DataFrames to optimize repeated computations.

Join with other datasets for enrichment (e.g., orders, transactions).

Apply window functions for ranking or running totals.

Tools and Technologies

Apache Spark (PySpark)

HDFS (or local filesystem for testing)

Python 3.x

Outcome

A reproducible batch ETL pipeline for customer data.

Aggregated insights suitable for analytics and reporting.

Foundation for extending to streaming pipelines, workflow orchestration with Airflow, and cloud integration in the future.

How to Run

Start Spark session with your cluster or local Spark setup.

Place the raw dataset in HDFS or local folder.

Execute the ETL pipeline script step by step: ingestion, cleaning, transformation, aggregation, and export.

Verify outputs and explore results.
