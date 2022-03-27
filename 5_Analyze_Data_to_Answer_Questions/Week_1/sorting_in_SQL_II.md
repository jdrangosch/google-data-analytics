# Quiz
A data analyst wants to sort a list of greenhouse shrubs by price from least expensive to most expensive. Which statement should they use?

WHERE shrub_price ASC   
ORDER BY shrub_price DESC   
WHERE shrub_price   
ORDER BY shrub_price    

> To sort a list of greenhouse shrubs by price from least expensive to most expensive, they should use ORDER BY shrub_price.

You are working with a database table that contains data about music genres.
You want to sort the genres by name in ascending order. The genres are listed in the genre_name column. 

You write the SQL query below. Add an ORDER BY clause that will sort the genres by name in ascending order. 

```
SELECT 
*
FROM 
genre
ORDER BY genre_name
```
```
+----------+--------------------+
| genre_id | genre_name         |
+----------+--------------------+
|       23 | Alternative        |
|        4 | Alternative & Punk |
|        6 | Blues              |
|       11 | Bossa Nova         |
|       24 | Classical          |
|       22 | Comedy             |
|       21 | Drama              |
|       12 | Easy Listening     |
|       15 | Electronica/Dance  |
|       13 | Heavy Metal        |
|       17 | Hip Hop/Rap        |
|        2 | Jazz               |
|        7 | Latin              |
|        3 | Metal              |
|       25 | Opera              |
|        9 | Pop                |
|       14 | R&B/Soul           |
|        8 | Reggae             |
|        1 | Rock               |
|        5 | Rock And Roll      |
|       20 | Sci Fi & Fantasy   |
|       18 | Science Fiction    |
|       10 | Soundtrack         |
|       19 | TV Shows           |
|       16 | World              |
+----------+--------------------+
```
What genre appears in row 3 of your query result? 

Easy Listening    
Alternative   
Blues   
Classical   

> The clause ORDER BY genre_name will sort the genres by name in ascending order. The complete query is SELECT * FROM genre ORDER BY genre_name. The ORDER BY clause tells the database how to organize the data it returns. The ORDER BY clause sorts data in ascending order by default. 

> The Blues genre appears in row 3 of your query result. 

Question 3
You are working with a database table that contains employee data. You want to sort the employees by hire date in descending order. The hire dates are listed in the hire_date column. 

You write the SQL query below. Add an ORDER BY clause that will sort the employees by hire date in descending order. 

```
SELECT 
*
FROM 
employee
ORDER BY hire_date DESC
```

```
+-------------+-----------+------------+---------------------+------------+---------------------+---------------------+-----------------------------+------------+-------+---------+-------------+-------------------+-------------------+--------------------------+
| employee_id | last_name | first_name | title               | reports_to | birth_date          | hire_date           | address                     | city       | state | country | postal_code | phone             | fax               | email                    |
+-------------+-----------+------------+---------------------+------------+---------------------+---------------------+-----------------------------+------------+-------+---------+-------------+-------------------+-------------------+--------------------------+
|           8 | Callahan  | Laura      | IT Staff            |          6 | 1968-01-09 00:00:00 | 2004-03-04 00:00:00 | 923 7 ST NW                 | Lethbridge | AB    | Canada  | T1H 1Y8     | +1 (403) 467-3351 | +1 (403) 467-8772 | laura@chinookcorp.com    |
|           7 | King      | Robert     | IT Staff            |          6 | 1970-05-29 00:00:00 | 2004-01-02 00:00:00 | 590 Columbia Boulevard West | Lethbridge | AB    | Canada  | T1K 5N8     | +1 (403) 456-9986 | +1 (403) 456-8485 | robert@chinookcorp.com   |
|           5 | Johnson   | Steve      | Sales Support Agent |          2 | 1965-03-03 00:00:00 | 2003-10-17 00:00:00 | 7727B 41 Ave                | Calgary    | AB    | Canada  | T3B 1Y7     | 1 (780) 836-9987  | 1 (780) 836-9543  | steve@chinookcorp.com    |
|           6 | Mitchell  | Michael    | IT Manager          |          1 | 1973-07-01 00:00:00 | 2003-10-17 00:00:00 | 5827 Bowness Road NW        | Calgary    | AB    | Canada  | T3B 0C5     | +1 (403) 246-9887 | +1 (403) 246-9899 | michael@chinookcorp.com  |
|           4 | Park      | Margaret   | Sales Support Agent |          2 | 1947-09-19 00:00:00 | 2003-05-03 00:00:00 | 683 10 Street SW            | Calgary    | AB    | Canada  | T2P 5G3     | +1 (403) 263-4423 | +1 (403) 263-4289 | margaret@chinookcorp.com |
|           1 | Adams     | Andrew     | General Manager     |       None | 1962-02-18 00:00:00 | 2002-08-14 00:00:00 | 11120 Jasper Ave NW         | Edmonton   | AB    | Canada  | T5K 2N1     | +1 (780) 428-9482 | +1 (780) 428-3457 | andrew@chinookcorp.com   |
|           2 | Edwards   | Nancy      | Sales Manager       |          1 | 1958-12-08 00:00:00 | 2002-05-01 00:00:00 | 825 8 Ave SW                | Calgary    | AB    | Canada  | T2P 2T3     | +1 (403) 262-3443 | +1 (403) 262-3322 | nancy@chinookcorp.com    |
|           3 | Peacock   | Jane       | Sales Support Agent |          2 | 1973-08-29 00:00:00 | 2002-04-01 00:00:00 | 1111 6 Ave SW               | Calgary    | AB    | Canada  | T2P 5M5     | +1 (403) 262-3443 | +1 (403) 262-6712 | jane@chinookcorp.com     |
+-------------+-----------+------------+---------------------+------------+---------------------+---------------------+-----------------------------+------------+-------+---------+-------------+-------------------+-------------------+--------------------------+
```
What employee appears in row 1 of your query result?

Robert King   
Laura Callahan    
Nancy Edwards   
Margaret Park   

> The clause ORDER BY hire_date DESC will sort the employees by hire date in descending order. The complete query is SELECT * FROM employee ORDER BY hire_date DESC. The ORDER BY clause tells the database how to organize the data it returns. The ORDER BY clause sorts data in ascending order by default. The DESC command is used to sort data in descending order. 

> The employee Laura Callahan appears in row 1 of your query result. 
