# Quiz
Fill in the blank: In SQL, _____ can be used to combine strings from multiple tables in order to create a new string.

COMBINE   
CONCATENATE   
CONCAT    
CONNECT   

> In SQL, CONCAT can be used to combine strings from multiple tables in order to create a new string.

You are working with a database table that contains data about playlists for different types of digital media. You are only interested in the first 4 playlists. 

You write the SQL query below. Add a LIMIT clause that will return only the first 4 playlists. 

```
SELECT 
*
FROM 
playlist
LIMIT 4
```
```
+-------------+------------+
| playlist_id | name       |
+-------------+------------+
|           1 | Music      |
|           2 | Movies     |
|           3 | TV Shows   |
|           4 | Audiobooks |
+-------------+------------+
```

What playlist appears in row 2 of your query result?

Audiobooks    
Movies    
TV Shows    
Music   

> The clause LIMIT 4 will return only the first 4 playlists. The complete query is SELECT * FROM playlist LIMIT 4. The LIMIT clause sets a limit on the number of rows your query returns. 

> The Movies playlist appears in row 2 of your query result.

What function can be used to return the number of characters in cell B8 so you can confirm that it contains exactly 20 characters?

=LEN(20)    
=LEN(B8)    
=LEN(20, B8)    
=LEN(B8, 20)    

> The function =LEN(B8) will display the number of characters in cell B8. The LEN function returns the length of a string of text by counting the number of characters it contains.

