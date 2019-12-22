# Data Modelling with Postgres

## Introduction
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

They'd like a data engineer to create a Postgres database with tables designed to optimize queries on song play analysis, and bring you on the project. Your role is to create a database schema and ETL pipeline for this analysis. You'll be able to test your database and ETL pipeline by running queries given to you by the analytics team from Sparkify and compare your results with their expected results.

## Running the ETL 
python3 create_tables.py
python3 etl.py

## What does the python ETL applications(scripts) do?
The three main files are create_tables.py, sql_queries.py and etl.py. 
* create_tables.py: Clean previous schema and creates tables.
* sql_queries.py: All SQL queries used in the ETL pipeline.
* etl.py: Read JSON logs and JSON metadata and load the data into generated tables.

## Database Schema
<img src="DatabaseModel.png">

* songplays: Records in log data associated with song plays
* users: Users in the app
* songs: Songs in music database
* artists: Artists in music database
* time: Timestamps of records in songplays broken down into specific units

