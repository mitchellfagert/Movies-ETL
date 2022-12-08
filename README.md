# Movies-ETL
This is a project that showcases an Extract, Transform, Load (ETL) process to create data pipelines using Python, Pandas and PostgreSQL using very large data files.

![etl-banner](https://user-images.githubusercontent.com/107579508/206490779-ce1eaca6-a12c-4446-8166-b7f9c2eab190.jpg)

## Overview
The purpose of this project was to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables that is connected to a database. The chosen topic is all about Movies from 1990 to 2018 and combining the information from 3 different resources.

## Process
Create an ETL pipeline using Jupyter Notebooks and PostgreSQL from raw data to SQL database.

* **Extract:** read data from multiple sources using Python. Data sourced from:

  * **Wikipedia:** (format: .json, file size: 6.2MB) 7,311 thousand movie titles that include information about the movies, budgets, box office returns, cast/crew, production and distribution.
  * **Kaggle:** - 2 files (formate: .csv)
    *     metadata file from The Movie Database containing movie details with 45.5 thousand entries. (File size: 34.4MB)
    *     a dataset from MovieLens containing over 26 million movie ratings/review. (File size: 709.6MB)
 
* **Transform:** Clean and structure data using Pandas and regular expressions (RegEx) to achieve desired form. (i.e. using RegEx to parse data and transform text into numbers.

  *  Deleting bad data (corrupted or missing), removing duplicate rows, and consolidating columns.
  *  Using RegEx to parse data and transform text into numbers.
 
* **Load:** Export transformed data into a database.

## Results
I was able to extract, transform, and load the datasets as two new tables into PostgreSQL by using Python. The final results created a movies table with 6,052 rows. A 17% reduction from the original of 7,311 and a ratings table with 52,048,578 rows.
![Movies_count](https://user-images.githubusercontent.com/107579508/206494819-396b2a51-8a7a-410e-8d02-a2d9b145f56d.png)


