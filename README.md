# ETL_Harmony_Flow

## Problem Statement

+ In the healthcare industry, ensuring the timely and accurate processing of patient medical records is crucial for 
  providing high-quality care. However, healthcare facilities often face challenges in managing the vast amount of medical data generated daily, leading to inefficiencies in data processing and decision-making.

+ As a healthcare data engineer, you are tasked with designing and implementing an automated data pipeline to 
  streamline the ETL process for patient medical records. The goal is to extract medical data from diverse sources, transform it into a standardized format, and load it into a centralized database for analysis and reporting.

## Solution

+ This project offers a comprehensive solution utilizing Apache Airflow and Docker to automate the ETL process for 
  patient medical records. By leveraging these technologies, healthcare organizations can efficiently manage and analyze medical data, leading to improved patient care and operational efficiency.

## Key Features

### Airflow DAG for ETL

+ The python script defines tasks for extracting medical data from various sources, performing data cleansing and 
  transformation, and loading the processed data into a database. The DAG can be easily customized to accommodate different data sources and processing requirements.

### Dockerized Environment

+ The use of Docker and Docker Compose simplifies the deployment and management of the data pipeline. Docker 
  containers ensure consistency and reproducibility across different environments, facilitating seamless execution of the ETL process.

### Volume Mounting

+ Volume mounting is employed to synchronize data directories between Docker containers and the local machine. This 
  enables easy access to input data files, output files, and other resources used in the ETL process. By mounting volumes, healthcare organizations can securely store and manage sensitive medical data while ensuring accessibility and data integrity.

## Usage Instructions

### Setting Up the Environment:

+ Create a new directory named `healthcare_etl`.

```
    mkdir healthcare_etl
    cd healthcare_etl
```
+ Create a virtual environment in the `healthcare_etl` directory.

  ```
    python -m venv .venv
    source .venv/bin/activate
  ```
+ Running the ETL Pipeline:
+ Navigate to the `dags` directory and place the `recalls_etl_v1.py` script.

 ```
cd airflow/dags
 ```

+ Customize the DAG script (`medical_records_etl.py`) to suit your data processing requirements.

+ Access the Airflow UI to trigger the DAG and monitor the progress of the data pipeline.

```
airflow webserver --port 8080
```

### Querying the Data:

+ Validate the accuracy and completeness of the processed medical records by querying the database.
    
+ Utilize SQL queries to extract insights, generate reports, and support data-driven decision-making in healthcare 
  operations.

### Conclusion:

+ Our project offers a robust solution for automating the ETL process of patient medical records using Apache 
  Airflow, Docker, and volume mounting. By implementing this automated data pipeline, healthcare organizations can streamline data management, improve data quality, and enhance patient care delivery, ultimately leading to better healthcare outcomes.







