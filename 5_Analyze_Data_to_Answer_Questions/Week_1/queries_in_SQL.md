# Video Quiz
You are working on a project about music and have a table of genres you need to sort. The Genres table contains the columns GenreId and Name.

Write a SQL query to return the name of each genre from this table in alphabetical order.
```
SELECT Name FROM Genres ORDER BY Name
```
```
+--------------------+
| Name               |
+--------------------+
| Alternative        |
| Alternative & Punk |
| Blues              |
| Bossa Nova         |
| Classical          |
| Comedy             |
| Drama              |
| Easy Listening     |
| Electronica/Dance  |
| Heavy Metal        |
| Hip Hop/Rap        |
| Jazz               |
| Latin              |
| Metal              |
| Opera              |
| Pop                |
| R&B/Soul           |
| Reggae             |
| Rock               |
| Rock And Roll      |
| Sci Fi & Fantasy   |
| Science Fiction    |
| Soundtrack         |
| TV Shows           |
| World              |
+--------------------+
```

What are the first and last music genres returned, respectively? Separate your answers by a comma followed by a space.

> Alternative and World are returned when making the following query:

> SELECT Name FROM genres ORDER BY Name

> Not specifying ascending or descending in your query will sort by ascending order by default. This is appropriate for sorting in alphabetical order.
