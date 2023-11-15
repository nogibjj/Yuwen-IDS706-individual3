## Duke IDS 706 Data Engineering individual project # 3
---

Youtube Link: 
https://youtu.be/MJBjX9fHs8E

---

## Summary*

This individual project aims to create an ETL operations pipeline on a dataset in Databricks Azure.

Project Structure:

![structure](<img/str.jpeg>)


---
## Code Location

You can find the data processing notebook in the following files:
- `DATA ETL.ipynb`

This notebook performs Extract, Transform, and Load operations for a sample dataset in Databricks and uses Delta Lake for data storage.

---

## Preparations

1. Create a cluster in Databricks
2. Create a notebook in a workspace
3. Perform ETL operations
4. Setup a workflow and schedule an automated trigger

---

## Databricks Result

### Data ETL operations:
Use Spark SQL to transform data and configure Auto Loader to ingest JSON data to a Delta table

![DATA ETL](<img/data_etl.png>)

### Loaded Dataset:

![DATA LOADED](<img/data_loaded.png>)

### Delta Lake Validation Check:

Quality Check: Check for null values in the Delta table

![Validation Check](<img/validation_check.png>)

### Data Visualization:

Visualize the first 5000 records of data in every 10-second time interval to show the time series data trend.

![Data Visualization](<img/data_visualize.png>)

### Workflow and Automation Setup:

Since all the ETL and visualization operations are performed in one notebook, only one event is in the workflow.
Schedule the workflow in a daily manner.

![Workflow](<workflow.png>)




