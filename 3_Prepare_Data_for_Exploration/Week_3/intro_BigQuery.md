# Introduction to BigQuery
Run another query on your table:

```
SELECT end_station_name FROM `bigquery-public-data.london_bicycles.cycle_hire` WHERE rental_id = 57635395;
```
At what station did the bike trip with rental_id 57635395 end?

Southwark Street, Bankside
Notting Hill Gate Station, Notting Hill
East Village, Queen Elizabeth Olympic Park (C)
Tower Gardens, Tower

The address listed under the end_station_name column for Row 1 of your results table was East Village, Queen Elizabeth Olympic Park. To find this, you successfully ran a query. Going forward, you will continue using SELECT, FROM, and WHERE statements in your queries to interact with databases using SQL. This will help you build more complicated SQL queries when you are analyzing data in the future.

In this activity, you had an opportunity to get more familiar with BigQuery and writing SQL queries. In the text box below, write 2-3 sentences (40-60 words) in response to each of the following questions:

How do you think you can use public datasets on BigQuery to help develop your data analysis skills?

How do you think understanding basic query syntax will help you write more complicated queries in the future?

Public Data Sets and BigQ are great tools and information to create projects and start working with data analytics, and develop new skills.
I think the most important thing is not sintaxis, but logical thinking about the table, what you are looking for and how can you filter it. If you understand that the rest is sintaxis that you can look up always.

> Congratulations on completing this hands-on activity! You explored BigQuery, uploaded public data to your console, and constructed some queries. A good response would include that BigQuery public datasets can help you practice writing SQL.

> Being able to construct SQL queries is an important skill for data analysts, because they frequently need to work with databases. In upcoming activities, you will continue working with databases and writing queries with SQL-- an essential tool in every data analyst’s toolkit.




