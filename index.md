---
layout: default
title: Akshay Akula
---

# Akshay Akula

## About Me

As a Data Engineer at PayPal, I build and maintain data pipelines, data lakes, and dashboards using Google Cloud Platform (GCP) and coordinate tasks among the team. I also design and implement star schema in Big Query and use g-cloud functions with Python to load data from Google Cloud Storage (GCS) buckets. I have experience in migrating on-prem Hadoop systems to GCP and using cloud Dataflow, Dataproc, and Bigtable for big data processing.

I have a Master's degree in Computer Science from University of Central Missouri, where I learned the fundamentals of data science, machine learning, and artificial intelligence. Before joining PayPal, I worked as a Data Engineer at Marsh McLennan and Virtusa, where I designed and developed data architectures and ETL processes using AWS, Snowflake, Airflow, and PySpark. I also developed Tableau and Google Looker reports and dashboards for data visualization and analysis. I have multiple certifications in Google Cloud, SQL, and Confluence, and I have won several awards for my performance and innovation. I am passionate about learning new technologies and trends in the data science and AI field, and I enjoy mentoring, working, and learning from some of the best and brightest analytical minds and data scientists in the business.

- **email -** akshay.wsh@gmail.com
- [LinkedIn](https://www.linkedin.com/in/akshay-akula/)

## Professional Experience

In my eight years as a Data Engineer, I’ve cultivated a deep passion for data architecture, data management, ETL processes, and data analysis. My journey began at Etouch systems, where I honed my skills in writing complex SQL Queries, data visualization using Power BI and SQL. I excelled in utilizing MS Excel for complex data analysis, delivering actionable insights that resulted in a 90% client satisfaction rate.

My Data Engineer experience at Virtusa & Marsh McLennan was a pivotal experience in my career. I applied Agile methodologies to enhance ETL pipelines using Informatica, Spark, and Scala, reducing data processing errors by 50%. Additionally, I contributed to bolstering data security through Python scripts. My proficiency in cloud engineering, AWS EMR Glue Jobs and Power BI helped increase operational efficiency by 40%, as I played a key role in optimizing data workflows and integration strategies.

Currently, as a Data Architect & Data Engineer at Paypal, I oversee the data infrastructure to ensure seamless data management and processing. My role involves creating and managing automated data import/export jobs, optimizing databases with Big query, writing complex queries, and generating reports using Looker studio. I also design data pipelines end to end based on data requirement to meet internal business needs. I have experience in migrating on-prem Hadoop systems to GCP and using cloud Dataflow, Dataproc, and Bigtable for big data processing. Additionally, I integrate data from external APIs, leverage data modeling techniques, and contribute to database performance enhancements through monitoring and backup strategies, ensuring reliability and scalability.

## Projects

### Exploratory Data Analysis of Car

<!-- (https://www.dropbox.com/) -->

- I focused on data pre-processing to ensure the dataset was accurately formatted and ready for analysis. I conducted exploratory data analysis (EDA) to investigate the relationships between various car features and their market prices. Utilizing the "Car Features and MSRP" dataset from Kaggle, which encompasses nearly 12,000 car models sold in the USA from 1990 to 2017, I applied descriptive statistics and visualizations to uncover hidden insights and trends in the data, including both new and used market prices. This project enhanced my ability to extract valuable information from complex datasets and informed decision-making processes in the automotive domain.

### Exploring GCP Components for Data Ingestion & Analytics

<!-- (https://docs.google.com/document/d/1Dbr4yqm8TBcNwlgrQwQ5U9O_Um5PUcPjUG4OCIrgbwc/edit?tab=t.0) -->
- The overall objective is to ingest Yelp batch data from GCS to BigQuery through scheduling jobs in GCP Composer/Airflow using DAG’s and creating a data pipeline in Dataflow. The source data file format we receive to the GCS bucket is json files. We need to parse the json in the Dataflow template and load the data to BQ tables.

### Data Pipeline from AWS S3 to Snowflake using Airflow

- The project aims to develop a data pipeline to ingest batch data from AWS S3 into Snowflake by orchestrating jobs in GCP Composer (Airflow) through Directed Acyclic Graphs (DAGs). This pipeline will automate the process of parsing, loading, and transforming JSON files stored in S3 into Snowflake, ensuring data consistency and efficient storage.

   Data Ingestion from S3:
   Source data is received in JSON format and stored in AWS S3 buckets.
   The DAGs in Airflow initiate scheduled jobs to read these JSON files, parsing them within custom Python code.

   Loading Data into Snowflake:
   Initial Load: JSON data is initially loaded into Snowflake’s RAW tables to retain unprocessed information.
   Data Parsing and Module-based Extraction: Based on predefined criteria (e.g., "Individual" or "Admin" payload types), the parsed JSON files are extracted 
   and organized into respective S3 buckets by modules, using datetime identifiers for partitioning.

   Raw Table Management:
   After each batch processing, RAW tables are refreshed by deleting and recreating them. This ensures that data is not duplicated and is optimized for 
   storage 
   efficiency.JSON files from S3 buckets are reloaded into the Snowflake RAW tables, preparing them for further transformations.

   Transformation and Staging:
   The parsed data is inserted into Stage tables in Snowflake using Insert Overwrite logic. This approach consolidates the data for streamlined processing.
   After staging, the data undergoes further transformations, preparing it for final load into fact tables.

   Final Load into Fact Tables:
   A MERGE function is applied for an Upsert operation from Stage tables to Fact tables, utilizing primary key fields to manage data updates accurately.
   This final step ensures the fact tables contain the most current records, with historical data preserved as required.

   Outcome:
   By implementing this data pipeline, the project achieves a streamlined and automated workflow for loading JSON data into Snowflake, optimized for module- 
   based processing and efficient data management. The pipeline is designed for reliability and scalability, supporting diverse payload types and consistent 
   data integration across systems.



## Certifications

- [Google Cloud Professional Data Engineer](https://www.credential.net/91eb307e-0e3b-4513-9d37-fa17d2c75f36?key=a07bed8045110455891673b06dc8d9787468a34de58c022520160b55139fada9)
