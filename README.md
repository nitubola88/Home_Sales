# Module 22 Challenge: Home Sales Data Analysis

This repository contains the solution for the **Module 22 Challenge**, where we analyze home sales data using **SparkSQL**. The task involves reading, processing, and performing various queries on home sales data to determine key metrics.

## Challenge Overview

The challenge required analyzing the **home_sales_revised.csv** dataset and performing several tasks using **PySpark** and **SparkSQL**. These tasks included:

- Creating a PySpark DataFrame from the provided CSV file.
- Running SQL queries to calculate the average price for homes based on different conditions, such as number of bedrooms, bathrooms, square footage, etc.
- Caching and partitioning the data to optimize query performance.
- Comparing the performance of cached versus uncached queries.
- Creating and using Parquet-formatted data with partitioning.

## Tasks Completed

### 1. **Read Home Sales Data**
- Read the **home_sales_revised.csv** file from the AWS S3 bucket location into a PySpark DataFrame.

### 2. **Create a Temporary Table**
- Created a temporary table named `home_sales` from the PySpark DataFrame.

### 3. **SQL Queries**
- **Average Price of a Four-Bedroom House**: Calculated the average price of a four-bedroom house sold for each year.
- **Average Price of a Home Built with Specific Features**: Computed the average price of homes with three bedrooms, three bathrooms, and specific features, grouped by the year built.
- **Average Price Based on View Rating**: Determined the average price of homes based on the "view" rating, filtered for homes with an average price of $350,000 or more.
  
### 4. **Caching and Partitioning**
- Cached the `home_sales` temporary table for optimized performance.
- Compared the performance of queries before and after caching.
- Partitioned the data based on the `date_built` field and saved it in Parquet format.

### 5. **Uncaching and Verification**
- Uncached the `home_sales` table and verified that the table was no longer cached.
