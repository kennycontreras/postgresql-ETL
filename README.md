# PostgreSQL-ETL

PostgreSQL-ETL is an ETL project for an imaginary startup called Sparkify. This project create a database based on a star schema. There's 1 Fact table and 4 Dim tables.

All the raw data is stored in JSON Files. This project create an ETL pipeline to obtain all the information from JSON files with the help of pandas python library and insert the data into the database schema.

This app will allows the analytic team knows what songs are users listening to.

## Prerequisites

All libraries you need to install. I recommend you to use `pip install`

- psycopg2
- ipython-sql
- pandas
- numpy

## Getting Started

First of all, to run your ETL pipeline, we need to create the database. 
All the information about the database, create and insert statements  you can find it in **create_tables.py / sql_queries.py**

`python create_tables.py`

This will use all the information specified in your create_tables.py file, like username, password, database, and queries etc.
After that, will execute **CREATE STATEMENTS** for all your tables.

Now, it's time to execute your ETL pipeline. 

`python etl.py`

This ETL pipeline obtain all the information from JSON files, and insert the data based on requisities for the project and analytic team itself.
The data is procesed and filtered using pandas library which provide an amazing analytics functions to make sure that the data is ready to insert into the database.

All JSON files are located in `data` directory.








