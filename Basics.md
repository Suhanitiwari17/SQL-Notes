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
