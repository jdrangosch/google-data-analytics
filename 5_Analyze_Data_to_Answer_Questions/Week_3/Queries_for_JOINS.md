# Queries for JOINS
Before you join the two tables with queries, take a moment to review the various kinds of JOIN statements. 

The two most common kinds of JOIN statements are INNER JOINs and OUTER LEFT JOINs (also known simply as LEFT JOINs). As a review:

* INNER JOIN: Returns only the rows where the target appears in both tables. 

* LEFT JOIN: Returns every row from the left table, as well as any rows from the right table with matching keys found in the left table. 

Note the difference between the INNER JOIN and LEFT JOIN and the implications for when each should be used. Consider the following queries:
### Sintaxis

```
-- Let's say table_1 has 100 rows and table_2 has 10 rows.
-- They share 10 keys in common.

-- Using INNER JOIN --> We get 10 rows in our results.
SELECT
    COUNT(*)
FROM
    table_1
INNER JOIN
    table_2
ON table_1.key = table_2.key;

-- Using LEFT JOIN --> We get 100 rows in our results.
SELECT
    COUNT(*)
FROM
    table_1
LEFT JOIN
    table_2
ON table_1.key = table_2.key;
```

### Queries with JOINS and aliases
Now, it’s time to actually query the dataset. As a starting point, try a query that pulls information from both the international_education and country_summary tables. Copy, paste, and run the following query:

SELECT
'TABLE_LOCATION'.COLUMN
```
SELECT 
    `bigquery-public-data.world_bank_intl_education.international_education`.country_name, 
    `bigquery-public-data.world_bank_intl_education.country_summary`.country_code, 
    `bigquery-public-data.world_bank_intl_education.international_education`.value
FROM 
    `bigquery-public-data.world_bank_intl_education.international_education`
INNER JOIN 
    `bigquery-public-data.world_bank_intl_education.country_summary` 
ON `bigquery-public-data.world_bank_intl_education.country_summary`.country_code = `bigquery-public-data.world_bank_intl_education.international_education`.country_code
```

### Use descriptive aliases 
Try using descriptive aliases that tell you what they represent. This next query is the same query as the previous one, but with aliases to improve readability. Copy, paste, and run the following query: 
```
SELECT 
    edu.country_name,
    summary.country_code,
    edu.value
FROM 
    `bigquery-public-data.world_bank_intl_education.international_education` AS edu
INNER JOIN 
    `bigquery-public-data.world_bank_intl_education.country_summary` AS summary
ON edu.country_code = summary.country_code
```

### Confirmation and reflection 
In the last query, you use a LEFT JOIN instead of an INNER JOIN to find the correct information. Beneath the query results, you’ll find that the number of rows in your joined table is 281. If you rerun the query with an INNER JOIN instead of a LEFT JOIN, how many rows would it return?

274   
281   
301   
324   

> The number of rows returned by an INNER JOIN is 274. When you run the query with an INNER JOIN instead of a LEFT JOIN, you exclude universities without mascots and return fewer rows of data. Knowing which JOIN to use is very important for analyzing data. Going forward, you can use your knowledge of JOINs to properly combine data from multiple tables.

In this activity, you used JOIN statements to combine data from multiple tables. In the text box below, write 2-3 sentences (40-60 words) in response to each of the following questions.

Why do you think JOIN statements are important for working with databases? 

How do you distinguish INNER JOINS from OUTER JOINS?

Joins are a resourceful way to filter information from two tables and obtain a new table with summary information.
Inner Joins give a result "and" operator, meaning that objects must appear in both tables.
Outer Joins give a result "or" operator, meainng that object can appear in any table.
> Correct
> Congratulations on completing this hands-on activity! A good response would include that JOINs allow you to combine data from linked tables, which helps you make comparisons and answer business questions. 
> Mastering JOIN statements is one of the most important parts of SQL, as combining data from multiple database tables is a core skill for data analysts. And when you apply for jobs, remember that JOIN statements are a common topic in data analyst interviews! The more JOIN statements you write, the more prepared you will be for a data analyst role.






