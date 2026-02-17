## SQL Basics

## What is SQL?
SQL (Structured Query Language) is used to manage and query relational databases.

CREATE DATABASE temp1; -- create db
DROP DATABASE temp1; -- delete db

CREATE DATABASE college;
USE college;

CREATE TABLE student(
id INT PRIMARY KEY,
name VARCHAR(50),
age INT NOT NULL -- not null is a constraint
);

INSERT INTO student VALUES(0,"Suhani",20);
INSERT INTO student VALUES(1,"Mahek",21);

SELECT * FROM student;
