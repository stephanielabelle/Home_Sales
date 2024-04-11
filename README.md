# Utilizing SparkSQL for Home Sales Data Analysis 
  
## Objective  
To demonstrate how SparkSQL can effectively and efficiently analyze of home sales data in Google Colab.  

Google Colab script is available in the [Home_Sales_colab.ipynb](Home_Sales_colab.ipynb) file of this repository.  

### SparkSQL Effectiveness in Analysis  
SparkSQL queries were easily run to analyze average house prices over a variety of factors (number of bedrooms, number of bathroom, number of floors, build date, year of sale).  
SparkSQL is an effective tool to carry out data analysis.  
  
### Efficiency of Analysis
SparkSQL query runtime was determined across three data preparations:  
1. Initial temporary table creation  (1.43 seconds)  
2. Cache of temporary table  (0.94 seconds)  
3. Parquet formatting with partitions based on build date followed by temporary table creation  (0.81 seconds)  
  
As seen in the above runtimes, cache of the temporary table shortens query runtime compared to not caching.  Parquet formatting further shortens query runtime.  
  
## Conclusion  
SparkSQL is an effective tool for querying dataset, and has tools such as table caching and parquet formatting that allow for a more efficient analysis.  This would be especially useful for larger datasets.  
