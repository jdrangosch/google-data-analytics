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

You are working on a project about music and have a table of tracks you need to sort.

The database you use contains a Tracks table. The table contains the following columns: TrackId, Name, AlbumId, MediaTypeId, GenreId, Composer, Milliseconds, Bytes, and UnitPrice.

Write a SQL query to pull all columns from the Tracks table for only tracks with Chris Cornell as the composer. Sort the results in descending order by GenreId.

```
SELECT * FROM Tracks WHERE Composer = 'Chris Cornell' ORDER BY GenreId DESC
```

```
+---------+---------------------------+---------+-------------+---------+---------------+--------------+----------+-----------+
| TrackId | Name                      | AlbumId | MediaTypeId | GenreId | Composer      | Milliseconds |    Bytes | UnitPrice |
+---------+---------------------------+---------+-------------+---------+---------------+--------------+----------+-----------+
|    3388 | You Know My Name          |     270 |           2 |      23 | Chris Cornell |       240255 |  3940651 |      0.99 |
|    3387 | Disappearing Act          |     270 |           2 |      23 | Chris Cornell |       273320 |  4476203 |      0.99 |
|    3386 | Silence the Voices        |     270 |           2 |      23 | Chris Cornell |       267376 |  4379597 |      0.99 |
|    3385 | Finally Forever           |     270 |           2 |      23 | Chris Cornell |       217035 |  3565098 |      0.99 |
|    3384 | Your Soul Today           |     270 |           2 |      23 | Chris Cornell |       205959 |  3385722 |      0.99 |
|    3383 | Scar On the Sky           |     270 |           2 |      23 | Chris Cornell |       220193 |  3616618 |      0.99 |
|    3381 | Killing Birds             |     270 |           2 |      23 | Chris Cornell |       218498 |  3588776 |      0.99 |
|    3380 | Ghosts                    |     270 |           2 |      23 | Chris Cornell |       231547 |  3799745 |      0.99 |
|    3379 | She'll Never Be Your Man  |     270 |           2 |      23 | Chris Cornell |       204078 |  3355715 |      0.99 |
|    3378 | Safe and Sound            |     270 |           2 |      23 | Chris Cornell |       256764 |  4207769 |      0.99 |
|    3377 | Arms Around Your Love     |     270 |           2 |      23 | Chris Cornell |       214016 |  3516224 |      0.99 |
|    3376 | Poison Eye                |     270 |           2 |      23 | Chris Cornell |       237120 |  3890037 |      0.99 |
|    3375 | No Such Thing             |     270 |           2 |      23 | Chris Cornell |       224837 |  3691272 |      0.99 |
|    2522 | Bleed Together            |     203 |           1 |       1 | Chris Cornell |       232202 |  7597074 |      0.99 |
|    2520 | Blow Up The Outside World |     203 |           1 |       1 | Chris Cornell |       347898 | 11379527 |      0.99 |
|    2519 | Burden In My Hand         |     203 |           1 |       1 | Chris Cornell |       292153 |  9659911 |      0.99 |
|    2518 | Pretty Noose              |     203 |           1 |       1 | Chris Cornell |       253570 |  8317931 |      0.99 |
|    2517 | Fell On Black Days        |     203 |           1 |       1 | Chris Cornell |       282331 |  9256082 |      0.99 |
|    2515 | The Day I Tried To Live   |     203 |           1 |       1 | Chris Cornell |       321175 | 10507137 |      0.99 |
|    2514 | Spoonman                  |     203 |           1 |       1 | Chris Cornell |       248476 |  8289906 |      0.99 |
|    2513 | Rusty Cage                |     203 |           1 |       1 | Chris Cornell |       267728 |  8779485 |      0.99 |
|    2512 | Outshined                 |     203 |           1 |       1 | Chris Cornell |       312476 | 10274629 |      0.99 |
|    2508 | Loud Love                 |     203 |           1 |       1 | Chris Cornell |       297456 |  9660953 |      0.99 |
+---------+---------------------------+---------+-------------+---------+---------------+--------------+----------+-----------+
```

What is the name of the first track that the query returns?

> You Know My Name is the first value returned in the Name column when making the following query: 

> SELECT * FROM Tracks WHERE Composer='Chris Cornell' ORDER BY GenreId DESC 

> When executed, this query returns a list of tracks that were composed by Chris Cornell. The list would be sorted by GenreId in descending order.
