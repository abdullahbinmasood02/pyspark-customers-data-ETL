# Customer Data ETL Pipeline with PySpark

## Project Overview
This project demonstrates a batch ETL (Extract, Transform, Load) pipeline using **PySpark**. The pipeline processes a customer dataset, performing data cleaning, transformation, and aggregation to produce actionable insights. It is designed to run on distributed systems with **HDFS** or local storage, illustrating core data engineering concepts such as RDDs, DataFrames, and Spark SQL.

---

## Dataset
The dataset contains customer information with the following fields:

| Column Name         | Description                              |
|--------------------|------------------------------------------|
| customer_id         | Unique identifier for each customer      |
| name                | Customer name                            |
| city                | City of the customer                     |
| state               | State of the customer                    |
| country             | Country of the customer                  |
| registration_date   | Date the customer registered             |
| is_active           | Boolean indicating whether the customer is active |

Sample data:

| customer_id | name       | city  | state        | country | registration_date | is_active |
|-------------|------------|-------|-------------|---------|-----------------|-----------|
| 0           | Customer_0 | Pune  | Maharashtra | India   | 1/19/2023       | TRUE      |
| 1           | Customer_1 | Pune  | West Bengal | India   | 8/10/2023       | TRUE      |
| 2           | Customer_2 | Delhi | Maharashtra | India   | 8/5/2023        | TRUE      |
| 3           | Customer_3 | Mumbai| Telangana   | India   | 6/4/2023        | TRUE      |
| 4           | Customer_4 | Delhi | Karnataka   | India   | 3/15/2023       | FALSE     |

---

## Tools and Technologies
- Apache Spark (PySpark)
- HDFS (or local filesystem for testing)
- Python 3.x

---

## Outcome
- A reproducible batch ETL pipeline for customer data.
- Aggregated insights suitable for analytics and reporting.
- Foundation for extending to streaming pipelines, workflow orchestration, and cloud integration.

---

## How to Run
1. Start Spark session with your cluster or local Spark setup.
2. Place the raw dataset in HDFS or local folder.
3. Execute the ETL pipeline script step by step: ingestion, cleaning, transformation, aggregation, and export.
4. Verify outputs and explore results.

---

