# Module-22-Big-Data
This challenge requires using SparkSQL to determine key metric about home sales data. Once the data is developed, Spark will be used to create temporary views, partition data, cache and uncache a temporary table and verify that the table has been uncached.

## Steps
- Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
- Import the necessary PySpark SQL functions for this assignment.
- Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
- Create a temporary table called home_sales.
- Answer the following questions using SparkSQL:
    - What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
    - What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
    - What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
    - What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
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

## Results
-- The average price for a four-bedroom home by year , as shown in cell 22, is:
    - 2022: $296,363.88
    - 2021 $301,819.44
    - 2020: $298,353.78
    - 2019: $300,263.7

-- The average price for a three-bedroom, three-bath home rounded to two decimal places is:
   - 2017: $292,676.79
   - 2016: $290,555.07
   - 2015: $288,770.3
   - 2014: $290,852.27
   - 2013: $295,962.27
   - 2012: $293,683.19
   - 2011: $291,117.47
   - 2010: $292,859.62

-- The average price of a home for each year that has three bedrooms, three bathrooms, two floors, 
   and is greater than or equal to 2,000 square feet is:
 - 2017: $280,317.58
 - 2016: $293965.1
 - 2015: $297,609.97
 - 2014: $298,264.72
 - 2013: $303,676.79
 - 2012: $307,539.97
 - 2011: $276,553.81
 - 2010: $285,010.22

## Resources
In cells where year_built was involved, CoLab would not recognize the code as employed from examples from in-class activities. A querty to Chat GBT suggested that (TO.DATE) had to be added before (year_built). That resovled those sections of code.
