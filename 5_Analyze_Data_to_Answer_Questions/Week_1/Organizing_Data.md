# Quiz
Fill in the blank: A data analyst uses _____ to decide which data is relevant to their analysis and which data types and variables are appropriate.

database organization   
database relationships    
database normalization    
database references   

> Database organization enables analysts to make decisions about which data is relevant to pull for a specific analysis. It also helps them decide which data types and variables are appropriate.

A data analyst wants to organize a database to show only the 100 most recent real estate sales in Stamford, Connecticut. How can they do that?

The data analyst should add a filter to return only sales in Stamford, Connecticut, then sort the most recent sales at the top of their list.   
The data analyst should add a filter to return only sales in Stamford, Connecticut, then sort the least recent sales at the top of their list.    
The data analyst should filter out sales in Stamford, Connecticut, then sort the most recent sales at the top of their list.    
The data analyst should filter out sales in Stamford, Connecticut, then sort the least recent sales at the top of their list.   

> The data analyst should add a filter for only sales in Stamford, Connecticut, then sort the most recent sales at the top of their list.

You are working with a database table that contains customer data. The country column designates the country where each customer is located. You want to find out which customers are located in Brazil. 

You write the SQL query below. Add a WHERE clause that will return only customers located in Brazil. 
```
SELECT 
*
FROM 
customer
WHERE
country = 'Brazil'
Reset
```
```
+-------------+------------+-----------+--------------------------------------------------+---------------------------------+---------------------+-------+---------+-------------+--------------------+--------------------+-------------------------------+----------------+
| customer_id | first_name | last_name | company                                          | address                         | city                | state | country | postal_code | phone              | fax                | email                         | support_rep_id |
+-------------+------------+-----------+--------------------------------------------------+---------------------------------+---------------------+-------+---------+-------------+--------------------+--------------------+-------------------------------+----------------+
|           1 | Luís       | Gonçalves | Embraer - Empresa Brasileira de Aeronáutica S.A. | Av. Brigadeiro Faria Lima, 2170 | São José dos Campos | SP    | Brazil  | 12227-000   | +55 (12) 3923-5555 | +55 (12) 3923-5566 | luisg@embraer.com.br          |              3 |
|          10 | Eduardo    | Martins   | Woodstock Discos                                 | Rua Dr. Falcão Filho, 155       | São Paulo           | SP    | Brazil  | 01007-010   | +55 (11) 3033-5446 | +55 (11) 3033-4564 | eduardo@woodstock.com.br      |              4 |
|          11 | Alexandre  | Rocha     | Banco do Brasil S.A.                             | Av. Paulista, 2022              | São Paulo           | SP    | Brazil  | 01310-200   | +55 (11) 3055-3278 | +55 (11) 3055-8131 | alero@uol.com.br              |              5 |
|          12 | Roberto    | Almeida   | Riotur                                           | Praça Pio X, 119                | Rio de Janeiro      | RJ    | Brazil  | 20040-020   | +55 (21) 2271-7000 | +55 (21) 2271-7070 | roberto.almeida@riotur.gov.br |              3 |
|          13 | Fernanda   | Ramos     | None                                             | Qe 7 Bloco G                    | Brasília            | DF    | Brazil  | 71020-677   | +55 (61) 3363-5547 | +55 (61) 3363-7855 | fernadaramos4@uol.com.br      |              4 |
+-------------+------------+-----------+--------------------------------------------------+---------------------------------+---------------------+-------+---------+-------------+--------------------+--------------------+-------------------------------+----------------+
```

How many customers are located in Brazil? 

3   
9   
5   
7   

> The clause WHERE country = “Brazil” will return only customers located in Brazil. The complete query is SELECT * FROM customer WHERE country = “Brazil”. The WHERE clause filters results that meet certain conditions. The WHERE clause includes the name of the column, an equals sign, and the value(s) in the column to include. 

> There are 5 customers located in Brazil. 

