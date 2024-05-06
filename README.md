# Home Sales Data Analysis Project

## Project Overview
This project involves analyzing a dataset of home sales. The dataset includes various details about homes sold, such as the date built, price, number of bedrooms and bathrooms, square footage, number of floors, view rating, and more.

The goal of this project is to gain insights into the home sales data by running various queries using Apache Spark and PySpark SQL.

## Data
The data used in this project is stored in a CSV file hosted on an AWS S3 bucket. The file is read into a Spark DataFrame, which is then used for analysis.

## Tools Used
- **Apache Spark**: Used for big data processing and analysis.
- **PySpark SQL**: Used for running SQL queries on Spark DataFrames.
- **Parquet**: A columnar storage file format that is optimized for use with big data processing frameworks like Apache Spark.

## Analysis
The analysis includes calculating the average price of homes based on various factors such as the number of bedrooms, bathrooms, view rating, and more. The results are rounded to two decimal places for readability.

The project also involves comparing the runtime of queries on cached vs uncached data, and on data stored in different formats (CSV vs Parquet).

## Caching
Caching is used to optimize the performance of the application by keeping the most frequently accessed data in memory. The impact of caching on query runtime is explored in this project.

## Partitioning
The data is partitioned by the "date_built" field and written in Parquet format. The partitioned data is then read back into a DataFrame and used for analysis. The impact of partitioning on query runtime is explored in this project.

## Results
The results of the analysis are printed to the console. The runtime of each query is also printed to the console for comparison.

## Future Work
Future work could involve analyzing additional factors, using more complex queries, or exploring other optimization techniques in Spark.
