# Cleaning string variables using SQL
The tracks table contains the following columns: TrackId, Name, AlbumId, MediaTypeId, GenreId, Composer, Milliseconds, Bytes, and UnitPrice.

Create a query to return the TrackId, AlbumId, Composer and UnitPrice columns from this table.

```
SELECT TrackId, AlbumId, Composer, UnitPrice FROM tracks
```

```
+---------+---------+------------------------------------------------------------------------+-----------+
| TrackId | AlbumId | Composer                                                               | UnitPrice |
+---------+---------+------------------------------------------------------------------------+-----------+
|       1 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|       2 |       2 | None                                                                   |      0.99 |
|       3 |       3 | F. Baltes, S. Kaufman, U. Dirkscneider & W. Hoffman                    |      0.99 |
|       4 |       3 | F. Baltes, R.A. Smith-Diesel, S. Kaufman, U. Dirkscneider & W. Hoffman |      0.99 |
|       5 |       3 | Deaffy & R.A. Smith-Diesel                                             |      0.99 |
|       6 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|       7 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|       8 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|       9 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|      10 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|      11 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|      12 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|      13 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|      14 |       1 | Angus Young, Malcolm Young, Brian Johnson                              |      0.99 |
|      15 |       4 | AC/DC                                                                  |      0.99 |
|      16 |       4 | AC/DC                                                                  |      0.99 |
|      17 |       4 | AC/DC                                                                  |      0.99 |
|      18 |       4 | AC/DC                                                                  |      0.99 |
|      19 |       4 | AC/DC                                                                  |      0.99 |
|      20 |       4 | AC/DC                                                                  |      0.99 |
|      21 |       4 | AC/DC                                                                  |      0.99 |
|      22 |       4 | AC/DC                                                                  |      0.99 |
|      23 |       5 | Steven Tyler, Joe Perry, Jack Blades, Tommy Shaw                       |      0.99 |
|      24 |       5 | Steven Tyler, Joe Perry                                                |      0.99 |
|      25 |       5 | Steven Tyler, Joe Perry, Jim Vallance, Holly Knight                    |      0.99 |
+---------+---------+------------------------------------------------------------------------+-----------+
(Output limit exceeded, 25 of 3503 total rows shown)
```
What is the AlbumId of the 6th track? Please respond using a numeric value, i.e. enter '4' and not 'four'.

> One is the AlbumId of the 6th track returned when making the following query:

In a query, if you use the LENGTH, SUBSTR, or TRIM function in a WHERE clause, you can select data based on a string condition. If you are having trouble with these, you may need a refresher on how you created a WHERE clause with a numeric condition. The concept is the same, so try the following:

The invoices table contains the following columns: InvoiceId, CustomerId, InvoiceDate, BillingAddress, BillingCity, BillingState, BillingCountry, BillingPostalCode, Total.

Create a query to return the CustomerId, InvoiceDate and Total columns from this table for only invoice totals over $20.

```
SELECT
    CustomerId, InvoiceDate, Total 
FROM 
    invoices
WHERE
    Total > 20
```

```
+------------+---------------------+-------+
| CustomerId | InvoiceDate         | Total |
+------------+---------------------+-------+
|         45 | 2010-02-18 00:00:00 | 21.86 |
|         46 | 2011-04-28 00:00:00 | 21.86 |
|         26 | 2012-08-05 00:00:00 | 23.86 |
|          6 | 2013-11-13 00:00:00 | 25.86 |
+------------+---------------------+-------+
```

How many results are returned?

> Four results are returned when making the following query:
