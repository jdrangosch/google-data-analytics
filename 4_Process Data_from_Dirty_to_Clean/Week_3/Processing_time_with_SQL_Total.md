# Processing time with SQL
### Query a large dataset
You’ll now discover for yourself how these runtimes change with dataset size by running some queries on a huge dataset—Wikipedia!

1. Log in to BigQuery Sandbox. If you have a free trial version of BigQuery, you can use that instead. On the BigQuery page, click the Go to BigQuery button.

Note: BigQuery Sandbox frequently updates its user interface. The latest changes may not be reflected in the screenshots presented in this activity, but the principles remain the same. Adapting to changes in software updates is an essential skill for data analysts, and it’s helpful for you to practice troubleshooting. You can also reach out to your community of learners on the discussion forum for help.

2. If you have never created a BigQuery project before, click CREATE PROJECT on the right side of the screen. If you have created a project before, you can use an existing one or create a new one by clicking the project dropdown in the blue header bar and selecting NEW PROJECT.

3. Name your project something that will help you identify it later. You can give it a unique project ID or use an auto-generated one. Don’t worry about selecting an organization if you don’t know what to put.

4. Now, you’ll see the Editor interface. In the middle of the screen is a window where you can type code, and to the left is the Explorer menu where you can search for datasets.

5. Copy and paste the following query into the editor and run it. The formatting is just cosmetic, so don’t worry if it changes when copied over. The query should take 10-15 seconds to run:

```
SELECT language,title, SUM(views) AS views
FROM `bigquery-samples.wikipedia_benchmark.Wiki10B`
WHERE title LIKE '%Google%'
GROUP BY language,title
ORDER BY views DESC;
```
Note: This query sorts and filters a dataset. You don't need to understand each detail yet. Coming up, you will learn what each part of this query means and how to use its functions in your own work.

After the query finishes, your screen should appear like this:

```
1	en Google 9791779
2	es Google 2197268
3	en Google_Earth 1597374
4	en Google_Maps 1551982
5	en Google_Chrome 1079759
```
This query returns a table that displays the total number of times each Wikipedia page with “Google” in the title has been viewed in each language. Note the information that BigQuery provides on the query you just ran. As you can infer from the dataset’s title in the query, this dataset is a sample consisting of 10 billion rows from the Wikipedia public dataset. 

You’ll find that the query processes over 415 gigabytes of data when run—pretty impressive for 15 seconds! Note that if you run the query again, the runtime will be almost instant (as long as you haven’t changed the default caching settings). This is because BigQuery caches the query results to avoid extra work if the query needs to be rerun. 

### Confirmation and reflection
In your last query, you processed 415.8 GB of data. How many rows were returned by the query?

225,038
305,710
214,710
198,768

> The last query you ran returns 214,710 rows of data. At the bottom of the data preview, you can see how many rows you returned. Going forward, you can apply this knowledge of data size measurements to better understand how much data you will work with and what tool is best suited to each data analysis project.

In this activity, you compared the amount of time it takes to process different sizes of queries in SQL. In the text box below, write 2-3 sentences (40-60 words) in response to each of the following questions:

How did working with SQL help you query a larger dataset?

How long do you think it would take a team to query a dataset like this manually?

How does the ability to query large datasets in reasonable amounts of time affect data analysts?


It helped me query a very large data set in just 15 seconds, and produce a result.
Maybe days, weeks or months.
It is a great use of the technology, and having the ability to process gigabytes of data in few seconds is something really positive.

> Congratulations on completing this hands-on activity! A good response would include how querying a dataset with billions of items isn’t feasible without tools such as  relational databases and SQL.

> Performing large queries by hand would take years and years of manual work. The ability to query large datasets is an extremely helpful tool for data analysts. You can gain insights from massive amounts of data to discover trends and opportunities that wouldn’t be possible to find without tools like SQL. 

