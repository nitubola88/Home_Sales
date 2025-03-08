# Home Sales Data Analysis Challenge

## Overview
This project focuses on analyzing home sales data using **SparkSQL** in **Google Colab**. The tasks involve working with large datasets, optimizing performance with caching, partitioning data, running complex queries, and measuring the query runtime for efficiency comparisons.

## Project Tasks
1. **Load the Home Sales Data**: 
   - The dataset is loaded in multiple formats, including CSV and Parquet.

2. **Create Temporary Views**: 
   - A temporary view is created for both the CSV and Parquet formats to enable SQL queries on the data.

3. **Data Caching**: 
   - Data is cached for performance improvement, reducing the time required to run repeated queries.

4. **SQL Queries**: 
   - We ran various SQL queries to explore and analyze the data:
     - Query to calculate the average price of a home per "view" rating, rounding to two decimal places, and filtering for homes with a price greater than or equal to $350,000.

5. **Runtime Measurement**:
   - We measured the runtime of SQL queries and compared the performance of cached versus uncached queries to determine the efficiency improvements.

6. **Data Uncaching**: 
   - After completing the necessary queries, the home sales data was uncached to free up memory.

## Key Concepts
- **Caching**: Storing intermediate results in memory to speed up repeated operations.
- **Temporary Views**: Representations of tables that can be queried using SQL syntax.
- **Parquet and CSV Data Formats**: Efficient data storage formats for large datasets.
- **SQL Queries**: SQL syntax used to filter, group, and aggregate data for analysis.

## Results
- The average price of a home per "view" rating was calculated, showing a significant variance in home prices based on the "view" rating.
- Query runtimes were measured, with caching improving performance significantly in repeated queries.

## Technologies Used
- **Apache Spark**: Distributed computing framework for large-scale data processing.
- **Google Colab**: Cloud-based platform for running Python code and managing data analysis tasks.
- **SparkSQL**: SQL engine built on top of Apache Spark for querying structured data.
- **Parquet and CSV formats**: Data storage formats for efficient data loading and querying.

## Steps for Reproducibility
1. Clone the repository.
2. Load the required dataset into the notebook using Spark.
3. Execute the SQL queries as shown in the code.
4. Cache and uncache the data as required for performance optimization.
5. Measure and compare the runtimes for different queries.


