# Video Quiz Widely used SQL queries
The media_types table contains the following columns: MediaTypeId and Name.

Create a query to return the Name column from this table.
```
SELECT Name FROM media_types;
```
```
+-----------------------------+
| Name                        |
+-----------------------------+
| MPEG audio file             |
| Protected AAC audio file    |
| Protected MPEG-4 video file |
| Purchased AAC audio file    |
| AAC audio file              |
+-----------------------------+
```
What is the media type name of the 1st result returned? 
(Enter the exact name that appears in the table.)

> MPEG audio file is the media type name of the 1st result returned when making the following query:

The customers table contains the following columns: CustomerId, FirstName, LastName, Company, Address, City, State, Country, PostalCode, Phone, Fax, Email, SupportRepId.

Create a query to return the LastName and Country columns from this table for only customers in Germany.

```
SELECT LastName FROM customers WHERE Country = 'Germany'
```
```
+------------+
| LastName   |
+------------+
| Köhler     |
| Schneider  |
| Zimmermann |
| Schröder   |
+------------+
```
What is the last name of the customer for the 3rd result returned?

Zimmermann

> Great job. Zimmermann is the last name of the customer for the 3rd result returned when making the following query:
