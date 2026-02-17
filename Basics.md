## SQL Basics

## What is SQL?
SQL (Structured Query Language) is used to manage and query relational databases.

## Creating and dropping database
```sql
CREATE DATABASE temp1; -- create db
DROP DATABASE temp1; -- delete db
```

## Use Database
```sql
CREATE DATABASE college;
USE college;
```

## Create Table
```sql
CREATE TABLE table_name(
colname data_type,constraints,
colname data_type,constraints
);

CREATE TABLE student(
id INT PRIMARY KEY,
name VARCHAR(50),
age INT NOT NULL -- not null is a constraint
);
```
## Inserting values
```sql
INSERT INTO student VALUES(0,"Suhani",20);
INSERT INTO student VALUES(1,"Mahek",21);
```
## Showing table
```sql
SELECT * FROM student;
```
## Data types
char-can store char of fixed length(0-255)

varchar-can store char upto fixed length(0-255)

int , boolean , float , double

date = yyy-mm-dd

time (1901-2155)

## SQL Commands
DDL(Data Definition Language) - create ,alter,drop,rename,truncate

DQL(Data Query Language) - select

DML(Data Manipulation Lnguage) - insert,updat,delete

DCL(Data Control Language) - grant,revoke

TCL(Transaction Control Language) - start,commit,rollback

## If Not exists
```sql
CREATE DATABASE IF NOT EXISTS db_name;
DROP DATABASE IF EXISTS db_name;
SHOW DATABASES;
SHOW TABLES;
```
## Select and view all col
```sql
SELECT * FROM tab_name,
```

## Insert
```sql
INSERT INTO tab_name
(col1,col2)
VALUES
(col1_val1,col1_val2),
(col2_val1,col2_val2); -- order matter
```

## Keys
A Primary Key uniquely identifies each row in a table.It can not be NULL.

A Foreign Key is a column in one table that refers to the Primary Key of another table.
It creates a relationship between tables.

## Constraints
SQL Constraints are used to specify rules for data in a table.

NOT NULL - col cannot have null value.

UNIQUE - all values in col are different.

PRIMARY KEY - makes col unique and not null,but use only for one.

FOREIGN KEY - prevent action that would destroy link between tables.
```sql
.CREATE TABEL temp(
cust_id INT ,
FOREIGN KEY (cust_id) REFERENCES customer(id)
);
```

DEFAULT - set default value of col.

CHECK - it can limit the values allowed in a col.

## Select Basic Syntax

```sql
SELECT col1,col2 FROM tab_name;
SELECT * FROM tab_name; -- to select all
```
## WHERE Clause
```sql
SELECT col1,col2 FROM tab_name
WHERE conditions;
```
## Operators in Where clause
Arithmetic - +,-,*,/,%

Comparison - <,<=,>,>=,!=,==

Logical - AND,OR,NOT,IN BETWEEN,ALL,LIKE,ANY

Bitwise - &,|

```sql
SELECT * FROM student WHERE city IN ("Delhi","Mumbai"); -- (in -matches any value in the list)

SELECT * FROM student WHERE marks BETWEEN 80 AND 90; -- (both ranges are include in between)

SELECT * FROM student WHERE city NOT IN ("Delhi","Mumbai"); --(not in-to negate given condition)

SELECT * FROM student LIMIT 3; -- set upper limit on number of rows to be returned
```


