# Hands-On Activity: SQL sorting queries
### Load the dataset
1. Log in to BigQuery Sandbox. If you have a free trial version of BigQuery, you can use that instead. On the BigQuery page, click the Go to BigQuery button.

Note: BigQuery Sandbox frequently updates its user interface. The latest changes may not be reflected in the screenshots presented in this activity, but the principles remain the same. Adapting to changes in software updates is an essential skill for data analysts, and it’s helpful for you to practice troubleshooting. You can also reach out to your community of learners on the discussion forum for help.

2. If you have never created a BigQuery project before, click CREATE PROJECT on the right side of the screen. If you have created a project before, you can use an existing one or create a new one by clicking the project dropdown in the blue header bar and selecting NEW PROJECT.

3. Name your project something that will help you identify it later. You can give it a unique project ID or use an auto-generated one. Don’t worry about selecting an organization if you don’t know what to put.

4. Now, you’ll see the Editor interface. In the middle of the screen is a window where you can type code, and to the left is the Explorer menu where you can search for datasets.

5. Click + ADD DATA at the top of the Explorer menu, then Explore public datasets from the resulting dropdown.

6. In the Search Marketplace bar, type sdoh_cdc_wonder_natality.

7. Click the CDC Births Data Summary.

8. Click View Dataset. This will bring you back to the BigQuery Sandbox interface in a new tab.

Note: This may pin the bigquery-public-data dropdown to the Explorer menu. You can use this to browse datasets and tables.

9. Click back to the Editor tab. This is where you’ll use SQL during this activity.

### Combine ORDER BY with WHERE clauses

Next, modify the query so that it returns the top 10 counties with the highest birth counts for 2018 only. To do this, add a WHERE clause to the query that specifies only rows that have a Year value equal to 2018-01-01. Note how the ORDER BY clause comes after the WHERE clause. 

```
SELECT  
    *
FROM 
    `bigquery-public-data.sdoh_cdc_wonder_natality.county_natality`
WHERE
    Year = '2018-01-01'
ORDER BY 
    Births DESC
LIMIT 
    11
```

### Confirmation and reflection
The last query you ran returned the top 10 counties with the highest birth counts for 2018 only. Remove the LIMIT statement and run the query again. What is the county with the 11th highest birth count? 

Orange County, CA
Dallas County, TX
Unidentified Counties, KY
Miami-Dade County, FL

> The county with the 11th highest birth count in 2018 is Orange County, CA. To find this answer, you ran a query with an ORDER BY clause and a WHERE clause. Going forward, you can use this knowledge of SQL to better organize and structure your data.

In this activity, you practiced sorting data using SQL queries with ORDER BY and WHERE clauses. In the text box below, write 2-3 sentences (40-60 words) in response to each of the following questions:

How can the ORDER BY clause help you organize and structure your data?

Why is it helpful to use the ORDER BY and WHERE clauses together when sorting and filtering data?

Can you think of a business question that you could answer using this method?

SQL commands are really powerful tools to sort, and filter databases.
Sorting and filtering Data are escencial tools in the Data Analytics pocket that are used every single day.
If you have the right Data of course you can Query it and find answers.

> Congratulations on completing this hands-on activity! A good response would include that sorting the data you return in your queries is a crucial tool for analyzing and understanding data.

> You can also answer business questions by sorting the dataset according to a given metric. For instance, a store may want to know which products they sell the most or least. Sorting helps you answer business questions that involve phrases such as “how much,” “how many,” “best,” or “worst”—which will be a valuable skill in your career as a data analyst.




