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
