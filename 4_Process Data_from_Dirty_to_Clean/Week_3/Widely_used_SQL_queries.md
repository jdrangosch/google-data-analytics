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

> Great job. Zimmermann is the last name of the customer for the 3rd result returned when making the following query:.

### Insert new row in DB
Example of inserting new data in a DB
Sintaxis    
```
INSERT INTO 'data_base_location'
  (colum_1, colum_2, colum_3, ...) 
VALUES
  (Value_1, Value_2, Value_3, ...)
```
Example
```
INSERT INTO 'customer_data.customer_address'
  (customer_id, address, city, state, zipcode, country) 
VALUES
  (2645, '333 SQL Road', 'Jackson', 'MI', 49202, 'US')
```
### Update field in DB
Example of updating new data in a DB
Sintaxis    
```
UPDATE 'data_base_location' 
SET colum_1 = 'value_1'
WHERE colum_2 = 1234
```
Example
```
UPDATE 'data_base_location' 
SET address = '123 new adress'
WHERE customer_id = 2645

```


