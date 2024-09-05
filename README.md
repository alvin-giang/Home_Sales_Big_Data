# Home Sales Big Data Analysis
This project uses Apache Spark to analyze home sales data. It demonstrates how to perform complex queries on large datasets, utilize caching for performance improvement, and manage data partitioning for more efficient queries. The dataset is loaded from an AWS S3 bucket, and results are calculated using Spark SQL.

### Project OVerview

This project focuses on analyzing a home sales dataset using PySpark and Spark SQL. The dataset is loaded from an AWS S3 bucket, and various SQL queries are performed to derive insights such as average home prices based on different criteria. Additionally, the project showcases the benefits of caching, partitioning, and using Parquet formatted data for optimized querying.

Key tasks include:

* Loading and displaying data from AWS S3.
* Performing SQL queries to calculate average home prices based on features like the number of bedrooms, bathrooms, views, and square footage.
* Caching the data and comparing query runtimes with and without caching.
* Partitioning the data by `date_built` and saving it as Parquet files for efficient querying.

### Features

* **Data Loading**: Load data from an AWS S3 bucket directly into a Spark DataFrame.
* **SQL Queries**: Perform complex SQL queries on the dataset, including grouping and filtering based on home features.
* **Caching**: Use Spark's caching mechanism to speed up query execution and compare runtimes.
* **Data Partitioning**: Partition the dataset by `date_built` and store it as Parquet files for optimized querying.
* **Performance Measurement**: Track query runtimes and compare the performance of cached vs. non-cached data.

### Technologies Used

* **Apache Spark**: For distributed data processing and SQL querying.
* **PySpark**: Python API for Spark.
* **AWS S3**: Source for home sales data.
* **Parquet**: Columnar storage format for efficient querying and storage.
* **Python**: Programming language used for running the queries.

### Installation

1. Clone the repository:
```python
git clone https://github.com/alvin-giang/Home_Sales_Big_Data.git
```
2. Nevigate to the project folder:
```python
cd Home_Sales_Big_Data
```
3. Set up Apache Spark and PySpark in your environment:
    * Install PySpark:
    ```python
    pip install pyspark
    ```
4. Run the script in your environment.

### Repository Structure

* **home_sales_partitioned**: contains Parquet files for optimized querying.
* **Home_Sales**: contains main code.
* **LICENSE.txt**: contains license of the repository.
* **README.md**: contains overview of the repository.

### Usage

* Load the home sales data from the AWS S3 bucket and create a DataFrame.
* Run SQL queries to analyze the data, such as calculating the average home prices based on bedrooms, bathrooms, and other features.
* Cache the data to speed up query execution and compare runtimes.
* Partition the data by `date_built` and store it as Parquet files for optimized future queries.

#### Example Queries

* Average price of a four-bedroom house per year.
* Average price of homes with three bedrooms and three bathrooms per year built.
* Average price of homes based on view ratings, with a price greater than or equal to $350,000.
* Compare runtimes of cached vs. non-cached data.

### License

This project is licensed under the MIT License. See the `LICENSE.txt` file for details.