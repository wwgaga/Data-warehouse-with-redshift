# Project-Data-warehouse-with-redshift

The project is to set up data warehouse for Sparkify, a music streaming startup, to efficiently store and organize user activity and song metadata data retrieved from Amazon S3, using Amazon Redshift..
•	Create fact and dimension tables user activity and song metadata data for the star schema in Redshift.
•	Develop a ETL pipeline that extracts their data from S3, stages them in Redshift, and transforms data into a set of dimensional tables
•	Design a star schema tailored for efficient SQL queries, particularly focused on song play analysis.

## Introduction 

This repository contains the code and documentation for setting up a data warehouse for Sparkify, a music streaming startup, using Amazon Redshift. The data warehouse is designed to store and organize Sparkify's user activity and song metadata data from Amazon S3, enabling the analytics team to derive valuable insights.

## Project Overview
As a data engineer for Sparkify, the task is to build an ETL (Extract, Transform, Load) pipeline to:

1. Extract data from JSON logs containing user activity on the app.
2. Extract data from JSON metadata about songs in the app.
3. Stage this data in Amazon Redshift.
4. Transform the data into a set of dimensional tables optimized for analytics.
5. Enable the analytics team to gain insights into user behavior and song preferences.

## ETL Process
The ETL process consists of the following steps:

1.Create staging tables in Redshift to temporarily store the raw data from S3.
2.Copy data from S3 into the staging tables.
3.Create dimensional tables for songplays, users, songs, artists, and time.
4.Transform and insert data from staging tables into the dimensional tables.
5.Perform data quality checks to ensure data integrity.

## Project Structure
The project directory structure is organized as follows:

- 'create_tables.py': Python script to create the necessary tables in Redshift.
-'etl.py': Python script to perform ETL tasks, including data extraction, transformation, and loading.
-'sql_queries.py': SQL queries used to create tables, load data, and perform transformations.
- 'dwh.cfg': Configuration file containing Redshift and S3 bucket details.
- 'README.md': This readme file.
