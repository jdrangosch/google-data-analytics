# Analyze weather data in BigQuery
Previously, you learned how to use BigQuery to clean data and prepare it for analysis. Now you will query a dataset and save the results into a new table. This is a useful skill when the original data source changes continuously and you need to preserve a specific dataset for continued analysis. It’s also valuable when you are dealing with a large dataset and know you’ll be doing more than one analysis using the same subset of data. 

In this scenario, you’re a data analyst at a local news station. You have been tasked with answering questions for meteorologists about the weather. You will work with public data from the National Oceanic and Atmospheric Administration (NOAA), which has data for the entire United States. This is why you will need to save a subset of the data in a separate table. 

By the time you complete this activity, you will be able to use SQL queries to create new tables when dealing with complex datasets. This will greatly simplify your analysis in the future.

# Querying the data
The meteorologists who you’re working with have asked you to get the temperature, wind speed, and precipitation for stations La Guardia and JFK, for every day in 2020, in descending order by date, and ascending order by Station ID. Use the following query to request this information:

```
SELECT 
    AVG(temperature) AS Avg_Temp,
    AVG(wind_speed) AS Avg_Wind,
    AVG(precipitation) AS Avg_Precip,
FROM 
    `dummy-proyect-123.Wheater.NY_Wheater` 
WHERE
    date BETWEEN '2020-01-01' AND '2020-12-31'
```
Results
```
Avg_Temp	  Avg_Wind	  Avg_Precip
57.169945   9.557240  0.116352
```
### Confirmation and reflection

What was the average temperature at JFK and La Guardia stations between June 1, 2020 and June 30, 2020? 

72.883    
74.909    
92.099    
87.671    

> The average was 72.883. To find out the average temperature during this time period, you successfully created a new table using a query and ran another query against that table. Going forward, you will be able to use this skill to create tables with specific subsets of your data to query. This will help you draw insights from multiple data sources in the future.

In the text box below, write 2-3 sentences (40-60 words) in response to each of the following questions:

How can creating tables from queries help you perform data analysis in the future?

Why is being able to view specific subsets of a dataset important?

Large sets can be intimidating, so creating samples or filtering data is important to keep focus on the task ahead.
It is important to only focus on the Data to answer the question you need.

> Congratulations on completing this hands-on activity! In this activity, you explored two public datasets and created a new table using a query. A good response might include that creating tables using your queries allows you to work with a subset of data without changing the original. 

> For instance, now you can query weather data from just the weather stations in New York that you need. This is important for finding trends within a subset of data. In upcoming activities, you will continue analyzing data like this. 

