# Home Sales Analysis with PySpark

## Overview:

In this project, I analyze home sales data using PySpark. The project is structured to cover the creation of Spark DataFrames, temporary tables, and execution of SparkSQL queries to answer specific questions regarding home prices, characteristics, and performance.

## Project Steps:

### 1. Data Preparation:

- Imported necessary PySpark SQL functions.
- Read the 'home_sales_revised.csv' data into a Spark DataFrame.
- Created a temporary table named 'home_sales'.

### 2. SparkSQL Queries:

1. **Average Price for a Four-Bedroom House:**
   - Query to calculate the average price for a four-bedroom house sold for each year, rounded to two decimal places.

2. **Average Price of a Home with Specific Characteristics:**
   - Query to find the average price of homes with three bedrooms and three bathrooms for each year built, rounded to two decimal places.

3. **Average Price of Homes with Specific Features:**
   - Query to determine the average price of homes with three bedrooms, three bathrooms, two floors, and an area greater than or equal to 2,000 square feet for each year built, rounded to two decimal places.

4. **View Rating for Expensive Homes:**
   - Query to identify the "view" rating for homes costing more than or equal to $350,000, with runtime measurement.

### 3. Caching and Performance Comparison:

1. **Caching:**
   - Cached the temporary table 'home_sales'.
   - Checked if the temporary table is cached.

2. **Query Performance - Cached vs. Uncached:**
   - Ran the view rating query on the cached temporary table and computed the runtime.
   - Partitioned the dataset by the 'date_built' field and created a temporary table for the formatted parquet data.

3. **Parquet Data Query Performance:**
   - Ran the view rating query on the parquet temporary table and computed the runtime.

4. **Uncaching:**
   - Uncached the 'home_sales' temporary table.
   - Verified that the temporary table is uncached.

### 4. Repository Structure:

- The notebook 'Home_Sales.ipynb' contains all the code and queries.
- The GitHub repository is named 'Home_Sales' and hosts the project files.


