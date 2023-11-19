# Home Sales Analysis with SparkSQL
This project uses SparkSQL to analyze home sales data. The key tasks performed include creating temporary views, partitioning data, caching and uncaching a temporary table, and verifying the uncaching of the table.  All SparkSQL was written in the `Home_sales_colab.ipynb` file and developed using Google Colab.

## Analysis
Several questions were answered using SparkSQL:

- The average price for a four-bedroom house sold for each year was calculated.
- The average price of a home for each year it was built that has three bedrooms and three bathrooms was calculated.
- The average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet was calculated.
- The “view” rating for homes costing more than or equal to $350,000 was determined.
## Caching
1. The temporary table `homes` was cached.
2. The caching of the temporary table was verified.

## Partitioning
1. The data was partitioned by the “date_built” field on the formatted parquet home sales data.
2. A temporary table for the parquet data was created.
3. The query that filters out the view ratings with an average price of greater than or equal to $350,000 was run again. The runtime was determined and compared to the uncached runtime.
## Uncaching
1. The home_sales temporary table was uncached.
2. The uncaching of the home_sales temporary table was verified using PySpark.
