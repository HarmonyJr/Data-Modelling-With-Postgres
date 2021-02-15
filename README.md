# Introduction

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app. Once created, the database would provide Sparkify with the capability to analyse and gain more insights from the song and user activity data they have been collecting. 

The project contains the songs and user activity JSON log files and python scripts. The log_data JSON log files contains the information on the user activities and the song_data JSON log files contains information on the songs. To load the files into the tables, follow the steps below.


#### Project Files

* data folder - The folder contains the song_data and log_data subfolders. The song_data folder contains the song_data JSON logs which contain information on the songs. The log_data folder contains the user activity logs which contain information on the user activities. 

* sql_queries.py - Contains all SQL queries, and is imported into the last three files above. 

* create_tables.py - Drops and creates tables. Running this file resets the tables before each time we run ETL scripts.

* etl.ipynb - Reads and processes a single file from song_data and log_data and loads the data into our tables.

* etl.py - Reads and processes a single file from song_data and log_data and loads the data into our tables. We'll fill this based on ETL notebook.

* test.ipynb - Displays the first few rows of each table to let us check our database. 


#### Steps To Read and Load Data 

* Execute the create_tables python script to create the sparkifydb database, which other files links to.
* Execute the etl process to create the tables, read data from the log files and load the data into newly created tables.
* Execute the test file on the Jupyter Notebook to see the loaded data. 