# Module-22-Big-Data
This challenge requires using SparkSQL to determine key metric about home sales data. Once the data is developed, Spark will be used to create temporary views, partition data, cache and uncache a temporary table and verify that the table has been uncached.

## Steps
- Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
- Import the necessary PySpark SQL functions for this assignment.
- Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
- Create a temporary table called home_sales.
- Answer the following questions using SparkSQL:
    - What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
    - What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off          your answer to two decimal places.
    - What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater         than or equal to 2,000 square feet? Round off your answer to two decimal places.
    - What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and         round off your answer to two decimal places.
- Cache your temporary table home_sales.
- Check if your temporary table is cached.
- Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to   
  $350,000. Determine the runtime and compare it to uncached runtime.
- Partition by the "date_built" field on the formatted parquet home sales data.
- Create a temporary table for the parquet data.
- Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the   
  runtime and compare it to uncached runtime.
- Uncache the home_sales temporary table.
- Verify that the home_sales temporary table is uncached using PySpark.
- Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository. (Filed sent directly to GitHub 
  from CoLab).

## Resources
In cells where year_built was involved, CoLab would not recognize the code as employed from examples from in-class activities. A querty to Chat GBT suggested that (TO.DATE) had to be added before (year_built). That resovled those sections of code.
