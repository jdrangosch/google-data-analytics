# Quiz
Which of the following SQL functions can data analysts use to clean string variables? Select all that apply. 

LENGTH
COUNTIF 
TRIM
SUBSTR

> Data analysts can use the SUBSTR and TRIM functions to clean string variables. 

You are working with a database table that contains data about playlists for different types of digital media. The table includes columns for playlist_id and name. You want to remove duplicate entries for playlist names and sort the results by playlist ID. 

You write the SQL query below. Add a DISTINCT clause that will remove duplicate entries from the name column. 

NOTE: The three dots (...) indicate where to add the clause.

```
SELECT DISTINCT name
FROM
playlist
ORDER BY
playlist_id
```
```
+----------------------------+
| name                       |
+----------------------------+
| Music                      |
| Movies                     |
| TV Shows                   |
| Audiobooks                 |
| 90’s Music                 |
| Music Videos               |
| Brazilian Music            |
| Classical                  |
| Classical 101 - Deep Cuts  |
| Classical 101 - Next Steps |
| Classical 101 - The Basics |
| Grunge                     |
| Heavy Metal Classic        |
| On-The-Go 1                |
+----------------------------+
```

What playlist name appears in row 6 of your query result? 

Movies    
TV Shows    
Music Videos    
Audiobooks    

The clause DISTINCT name will remove duplicate entries from the name column. The complete query is SELECT DISTINCT name FROM playlist ORDER BY playlist_id. The DISTINCT clause removes duplicate entries from your query result. The playlist name Music Videos appears in row 6 of your query result. 

You are working with a database table that contains data about music albums. The table includes columns for album_id, title, and artist_id. You want to check for album titles that are less than 4 characters long. 

You write the SQL query below. Add a LENGTH function that will return any album titles that are less than 4 characters long.

```
SELECT 
  *
FROM
  album
WHERE
  LENGTH(title) < 4
```
```
+----------+-------+-----------+
| album_id | title | artist_id |
+----------+-------+-----------+
|      131 | IV    |        22 |
|      181 | Ten   |       118 |
|      182 | Vs.   |       118 |
|      236 | Pop   |       150 |
|      239 | War   |       150 |
+----------+-------+-----------+
```
What album ID number appears in row 3 of your query result? 

182   
131   
236   
239   

> The function LENGTH(title) < 4 will return any album names that are less than 4 characters long. The complete query is SELECT * FROM album WHERE LENGTH(title) < 4. The LENGTH function counts the number of characters a string contains. The album ID number 182 appears in row 3 of your query result. 

You are working with a database table that contains customer data. The table includes columns about customer location such as city, state, and country. You want to retrieve the first 3 letters of each country name. You decide to use the SUBSTR function to retrieve the first 3 letters of each country name, and use the AS command to store the result in a new column called new_country. 

You write the SQL query below. Add a statement to your SQL query that will retrieve the first 3 letters of each country name and store the result in a new column as new_country. 

NOTE: The three dots (...) indicate where to add the statement.

```
SELECT 
customer_id,
SUBSTR(country,1,2) AS new_country
FROM
customer
ORDER BY
country
```
```
+-------------+-------------+
| customer_id | new_country |
+-------------+-------------+
|          56 | Ar          |
|          55 | Au          |
|           7 | Au          |
|           8 | Be          |
|           1 | Br          |
|          10 | Br          |
|          11 | Br          |
|          12 | Br          |
|          13 | Br          |
|           3 | Ca          |
|          14 | Ca          |
|          15 | Ca          |
|          29 | Ca          |
|          30 | Ca          |
|          31 | Ca          |
|          32 | Ca          |
|          33 | Ca          |
|          57 | Ch          |
|           5 | Cz          |
|           6 | Cz          |
|           9 | De          |
|          44 | Fi          |
|          39 | Fr          |
|          40 | Fr          |
|          41 | Fr          |
+-------------+-------------+
```
What customer ID number appears in row 2 of your query result? 

47    
55    
28    
3   

> The statement SUBSTR(country, 1, 3) AS new_country will retrieve the first 3 letters of each state name and store the result in a new column as new_country. The complete query is SELECT customer_id, SUBSTR(country, 1, 3) AS new_country FROM customer ORDER BY country. The SUBSTR function extracts a substring from a string. This function instructs the database to return 3 characters of each country, starting with the first character. The customer ID number 55 appears in row 2 of your query result.  
