## Reddit Data Extraction, Transformation and Analysis

## Comprehensive Data Pipeline Implementation for Reddit Using Airflow, Celery, PostgreSQL, S3, AWS Glue, Athena, and Redshift

This initiative presents a detailed solution for extracting, transforming, and loading (ETL) data from Reddit into a Redshift data warehouse. It utilizes an array of technologies and services such as Apache Airflow, Celery, PostgreSQL, Amazon S3, AWS Glue, Amazon Athena, and Amazon Redshift to facilitate the data pipeline process.

## Project Summary
 
 This data pipeline aims to:

1. Retrieve data from Reddit through its API.
2. Deposit the unprocessed data into an S3 bucket via Airflow.
3. Process the data with AWS Glue and Amazon Athena.
4. Import the processed data into Amazon Redshift for analysis and querying purposes.


## System Design

1. Reddit API: The primary data source.
2. Apache Airflow & Celery: Coordinates the ETL activities and handles task allocation.
3. PostgreSQL: Serves as temporary storage for data and metadata handling.
4. Amazon S3: Stores the raw data.
5. AWS Glue: Manages the data catalog and performs ETL operations.
6. Amazon Athena: Facilitates SQL-based data processing.
7. Amazon Redshift: Used for data storage, analysis, and querying.


## Initial Requirements
1. An AWS account with necessary permissions for S3, Glue, Athena, and Redshift services.
2. Access credentials for the Reddit API.
3. Docker installed on your system.
4. Python version 3.9 or later"


## Run the project localy
1. Clone the repository.
   ```bash
    git clone https://github.com/airscholar/RedditDataEngineering.git
   ```
2. Create a virtual environment.
   ```bash
    python3 -m venv venv
   ```
3. Activate the virtual environment.
   ```bash
    source venv/bin/activate
   ```
4. Install the dependencies.
   ```bash
    pip install -r requirements.txt
   ```
5. Rename the configuration file and the credentials to the file.
   ```bash
    mv config/config.conf.example config/config.conf
   ```
6. Starting the containers
   ```bash
    docker-compose up -d
   ```
7. Launch the Airflow web UI.
   ```bash
    open http://localhost:8080
   ```


![image](https://github.com/aravinddudam/Reddit-Data-Extraction-Transformation-and-Analysis/assets/122600985/bc47e0bd-0cae-48c2-91b4-27cdc5fc7851)

   
