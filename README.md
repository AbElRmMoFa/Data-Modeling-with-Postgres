Introduction:
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app.
 The analytics team is particularly interested in understanding what songs users are listening to.
 Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

Project Description:
In this project, I will model the data with Postgres and build an ETL pipeline using Python.

Fact Table:

songplays records in log data associated with song plays

Dimension Tables:

users in the app

songs in music database

artists in music database

time: timestamps of records in songplays broken down into specific units


How to run the Python scripts :

in this project there is two jupyter notebooks etl and test :
 
the etl notebook purpose is to build the pipe lines step by step ,and the test is to findout if the rows inserted correctly or not.

and there is also three python scripts:

1-sql_queries.py where the tables syntax created as required in psycopg2 and also dropping the tables and a sql quary which will be used in the code  library and then imported in different scripts

2-create_tables.pt which simply make conncetion to the server and build or delete tables to be used late in ETL process.

3-etl.py which built  etl notebook but once you run it it would create the whole database




