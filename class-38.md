## Read 08

### SQL 

- Structured Query Language 
- designed to allow everyone to query and manipulate data

#### Relational databases
 - a collection of related (two dimensional tables)

 >`SELECT` will retrieve data
 >`FROM`  TTELLS IT WHERE TO SELECT FROM
 >`WHERE` helps filter data

 ### Filtering Queries

 >`DISTINCT` will blindly remove dupicate rows
 >`ORDER BY` will sort results in ASC or DESC order.
 >`LIMIT` will recudes result by how much you set it to
 >`OFFSET` will tell it where to start counting

 ### Insertign new data

 >`INSERT` statement will allow us to fill data into our table

 `INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;`


### Updateing values

`UPDATE mytable
SET column = value_or_expr, 
    other_column = another_value_or_expr, 
    …
WHERE condition;`

`UPDATE movies
SET director = "John Lasseter"
WHERE id = 2;`

#### Deleting

`DELETE FROM movies
where year < 2005;`

### Creating

`CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
);`

`CREATE TABLE Database (
    Name TEXT,
    Version FLOAT,
    Download_count INTEGER
);`