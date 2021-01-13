# SQL

## Intro to SQL

### What is SQL?

- Structured Query Language.
- Manipulate and transform data from a relational database.

### Relational databases

- A relational database represents a collection of related (two-dimensional) tables.


### SELECT queries 101

``` SELECT column, another_column, …
FROM mytable; ```

- ` SELECT * FROM mytable; ` * selects all columns and used as shorthand.

### Queries with constraints

- Using `WHERE` allows you to add condition for your queries to specify what you are looking for.
``` SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```
### Filtering and sorting Query results

- DISTINCT query will remove duplicate rows
- ORDER BY can be used to show results by either ASC/DESC
- LIMIT reduces number of rows to return
- OFFSET will specify where to begin counting rows from.

### Inserting rows

What is a Schema?

- In SQL, the *database* schema is what describes the structure of each table, and the datatypes that each column of the table can contain.
- INSERT statement is used to isnsert data into DB.
```
INSERT INTO mytable
VALUES (value_or_expr, another_value_or_expr, …),
       (value_or_expr_2, another_value_or_expr_2, …),
       …;
```
### Updating rows

- UPDATE statement can change existing data.
```
UPDATE mytable
SET column = value_or_expr, 
    other_column = another_value_or_expr, 
    …
WHERE condition;
```

### Deleteing rows

- DELETE can delete data from a table in DB
```
DELETE FROM mytable
WHERE condition;
```

### Creating tables

- CREATE TABLE create a new database table
```
CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
);
```

### Altering tables

- ALTER TABLE update correspoonding tables and DB to add, remove, modify columns and table constraints.
```
ALTER TABLE mytable
ADD column DataType OptionalTableConstraint 
    DEFAULT default_value;
```

### Dropping tables

- DROP TABLE removes entire table including all of its data and metadata




