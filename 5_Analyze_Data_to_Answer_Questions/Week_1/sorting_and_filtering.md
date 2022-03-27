# Video Quiz
You are working on an international project and need to invoice your customers for the work you complete. The database you use contains an invoices table. The invoices table contains the following columns: InvoiceId, CustomerId, InvoiceDate, BillingAddress, BillingCity, BillingState, BillingCountry, BillingPostalCode, Total.

Create a query to return all the columns from this table for only customers in Germany who have an invoice total greater than $5. 

Hint (if needed) - Your query should have the following structure:
SELECT _____
FROM   _____
WHERE _____  AND _____

```
SELECT CustomerId, InvoiceId, InvoiceDate, Total From invoices WHERE BillingCountry = 'Germany' AND Total > 5
```
```
+------------+-----------+---------------------+-------+
| CustomerId | InvoiceId | InvoiceDate         | Total |
+------------+-----------+---------------------+-------+
|          2 |        12 | 2009-02-11 00:00:00 | 13.86 |
|         36 |        40 | 2009-06-15 00:00:00 | 13.86 |
|         38 |        52 | 2009-08-08 00:00:00 |  5.94 |
|          2 |        67 | 2009-10-12 00:00:00 |  8.91 |
|         36 |        95 | 2010-02-13 00:00:00 |  8.91 |
|         37 |       138 | 2010-08-23 00:00:00 | 13.86 |
|         37 |       193 | 2011-04-23 00:00:00 | 14.91 |
|         38 |       236 | 2011-10-31 00:00:00 | 13.86 |
|          2 |       241 | 2011-11-23 00:00:00 |  5.94 |
|         36 |       269 | 2012-03-26 00:00:00 |  5.94 |
|         38 |       291 | 2012-06-30 00:00:00 |  8.91 |
|         37 |       367 | 2013-06-03 00:00:00 |  5.94 |
+------------+-----------+---------------------+-------+
```
How many rows are returned from this query?

12

> Twelve rows are returned when making the following query:

> SELECT * FROM invoices WHERE BillingCountry='Germany' AND Total > 5. 

> The AND clause allows you to write a query with more than one condition. This means that this query will return a list of 12 customers to charge that are from Germany and have invoices totaling more than $5.
