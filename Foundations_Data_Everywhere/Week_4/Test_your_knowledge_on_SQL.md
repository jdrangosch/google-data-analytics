# Quiz
&nbsp;
```
SELECT * FROM employee WHERE jobCode = 'FTE' AND LastName = 'James'
```

What does the asterisk (*) after SELECT tell the database to do in this query?

* Select, then delete data.
* Select and filter data.
* Select and multiply data.
* **Select all data.**

> The asterisk tells the database to select all data in the table.
&nbsp;

### Question 2

```
SELECT * FROM employee WHERE jobCode = 'FTE' AND LastName = 'James'
```

In this query, the data analyst wants to retrieve data from which table? 

* LastName
* **employee**
* James
* jobCode

> The data analyst wants to retrieve data from the employee table.
&nbsp;

### Question 3

```
SELECT * FROM employee WHERE jobCode = 'FTE' AND LastName = 'James'
```

In this query, the data analyst wants to retrieve all data from the employee table, where the jobCode is FTE and the last name is James.

* **True**
* False

> This query asks the database to select all data from the employee table, where the jobCode is FTE and the last name is James.
&nbsp;

### Question 4

You are writing a query and want to instruct the database to retrieve data from the warehouse_inventory table. What is the SQL statement that follows SELECT *? Type your answer below.

```
FROM warehouse_inventory
```

> The correct SQL statement is FROM warehouse_inventory. FROM indicates where the selected data comes from. And warehouse_inventory is the name of the table.

You are working with a database table that contains data about music artists. The table is named artist. You want to review all the columns in the table. 

You write the SQL query below. Add a FROM clause that will retrieve the data from the artist table.

```
SELECT * FROM artist
```
How many columns are in the artist table? 

9   
5   
8   
2 (Correct)   

> The clause FROM artist will retrieve the data from the artist table. The complete query is SELECT * FROM artist. The FROM clause specifies which database table to select data from. There are two columns in the artist table. 

You are working with a database table that contains data about music albums. You are only interested in data related to the album with ID number 277. The album IDs are listed in the album_id column from the album table.

You write the SQL query below. Add a WHERE clause that will return only data about the album with ID number 277.

```
SELECT * FROM artist WHERE album_id = '277'
```

What is the name of the album with ID number 277? 

Beethoven: Piano Sonatas    
Vivaldi: The Four Seasons   
Mozart: Chamber Music   
Bach: Goldberg Variations (Correct)   

> The clause WHERE album_id = 277 will return only data about the album with ID number 277. The complete query is SELECT * FROM album WHERE album_id = 277. The WHERE clause filters results that meet certain conditions. The WHERE clause includes the name of the column, an equals sign, and the value(s) in the column to include. The name of the album with ID number 277 is Bach: Goldberg Variations





