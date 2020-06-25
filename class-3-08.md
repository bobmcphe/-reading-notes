class-3-08.md

# SQL

## Intro

SQL stands for Structured Query Language, and while it is not a database itself, nor a way to store data, it is a means of accessing stored data on a database. These databases are relational databases and was designed by Donald D Chamberlin and Raymond F. Boyce. A relational database can be understood as a series of spreadsheets which interact with one another, these different spreadsheets, or tables, are interconnected.

Common SQL database softare would include MySQL, Postgres, Oracle, and even Microsoft Access.

## Cheat-sheet
### Database Manipulation
#### Create a database
CREATE DATABASE database_name	      
 
#### Delete a database
DROP DATABASE database_name	    
 
### Table Manipulation
 
####  Create a table in a database.
CREATE TABLE "table_name"
("column_1" "data_type_for_column_1",
"column_2" "data_type_for_column_2",
... )	     
 
### Data Manipulation
#### Insert new rows into a table.	
INSERT INTO table_name
VALUES (value_1, value_2,....)	      

#### Update one or several columns in rows.	
UPDATE table_name
SET column_name_1 = new_value_1, column_name_2 = new_value_2
WHERE column_name = some_value

#### Delete rows in a table.	
DELETE FROM table_name
WHERE column_name = some_value

#### Deletes the data inside the table.
TRUNCATE TABLE table_name

### Select
#### Select data from a table.
SELECT column_name(s) FROM table_name

#### Select all data from a table.	
SELECT * FROM table_name

#### Select only distinct (different) data from a table.
SELECT DISTINCT column_name(s) FROM table_name	

#### Select only certain data from a table.	
SELECT column_name(s) FROM table_name
WHERE column operator value
      AND column operator value
      OR column operator value
      AND (... OR ...)

## Select Operators
=	    Equal
<>	    Not equal
>	    Greater than
<	    Less than
>=	    Greater than or equal
<=	    Less than or equal
BETWEEN	    Between an inclusive range

For more information, see: http://www.cheat-sheets.org/sites/sql.su/