# Extract, Transform, Load Movie Data
## Overview
The purpose of this project is to gather the Wikipedia data, Kaggle metadata, and the Movielens rating data from Wekipedia and Kaggle website. However, the original data is not "flat data", firstly, we have to clean up the bad data. Then I used Python's pandas library to transform the data into a working dataframe. Finally, connected to PostgreSQL for analysis use.

## Process
There are 4 main parts of this process:
- write an ETL function to read three data files.
The function takes the Wikipedia JSON, the Kaggle metadata and MovieLens csv files and creates three separate DataFrames.
- extract and transform the Wikipedia data.
We filtered out the TV shows, consolidated the redundant data, removed the duplicates and formatted the Wikipedia data.
- extract and transform the Kaggle and rating data.
Again, we consolidated the redundant data, removed the duplicates, formatted and grouped the data.
The Kaggle and rating data were then merged with the Wikipedia movies DataFrame.
- load the data to a PostgreSQL Movie Database.

## Results
SQL screenshoot
