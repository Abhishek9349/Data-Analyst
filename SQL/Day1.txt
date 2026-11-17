==================================================
DAY 01 - SQL INTRODUCTION & DATABASE FUNDAMENTALS
==================================================

GOAL:
Understand SQL, databases, DBMS, RDBMS, tables, data types and basic SQL commands.

--------------------------------------------------
1. WHAT IS SQL?
--------------------------------------------------

SQL stands for Structured Query Language.

SQL is a programming language used to communicate with databases. It helps us store, retrieve, update and delete data.

Uses of SQL:
1. Find employees earning more than 30000.
2. Find employees working in the IT department.
3. Calculate average salary.
4. Find the highest-paid employee.
5. Count total employees.

Example:
SELECT * FROM employees;

This query retrieves all records from the employees table.

--------------------------------------------------
2. WHAT IS DATA?
--------------------------------------------------

Data means raw facts and information that can be processed.

Examples:
Name: Rahul
Age: 23
Salary: 25000
City: Delhi
Department: IT

When data is organized and processed, it becomes useful information.

--------------------------------------------------
3. WHAT IS A DATABASE?
--------------------------------------------------

A database is an organized collection of data that can be easily accessed, managed and updated.

Example:
A college database stores:
- Student details
- Teacher details
- Attendance
- Marks
- Fees

--------------------------------------------------
4. WHAT IS DBMS?
--------------------------------------------------

DBMS stands for Database Management System.

It is software used to create, store, manage and retrieve data from databases.

Examples:
- MySQL
- Oracle Database
- Microsoft SQL Server
- PostgreSQL
- SQLite

--------------------------------------------------
5. WHAT IS RDBMS?
--------------------------------------------------

RDBMS stands for Relational Database Management System.

It stores data in tables consisting of rows and columns. Different tables can be connected through relationships.

Example:

STUDENTS TABLE

Student_ID | Name  | Age
1          | Rahul | 22
2          | Priya | 23
3          | Amit  | 21

COURSES TABLE

Course_ID | Student_ID | Course
101       | 1          | BCA
102       | 2          | MCA
103       | 3          | BBA

Student_ID connects both tables.

--------------------------------------------------
6. IMPORTANT DATABASE TERMS
--------------------------------------------------

1. Table:
   Collection of related data.

2. Row:
   A single record in a table.

3. Column:
   An attribute or field.

4. Primary Key:
   Uniquely identifies each record.

5. Foreign Key:
   Connects two tables.

6. NULL:
   Represents missing or unknown data.

7. Schema:
   Structure of a database.

--------------------------------------------------
7. SQL DATA TYPES
--------------------------------------------------

Data types define what kind of data a column can store.

1. INT:
   Stores integer numbers.
   Example: 100

2. VARCHAR(n):
   Stores variable-length text.
   Example: Rahul

3. CHAR(n):
   Stores fixed-length text.
   Example: Male

4. DATE:
   Stores date values.
   Example: 2026-11-17

5. DECIMAL(p,s):
   Stores exact decimal numbers.
   Example: 25000.50

6. FLOAT:
   Stores approximate decimal numbers.
   Example: 25.5

7. BOOLEAN:
   Stores TRUE or FALSE values.

--------------------------------------------------
8. TYPES OF SQL COMMANDS
--------------------------------------------------

SQL commands are divided into five major categories.

1. DDL - Data Definition Language
   Defines database structure.
   Commands: CREATE, ALTER, DROP, TRUNCATE

2. DML - Data Manipulation Language
   Modifies data.
   Commands: INSERT, UPDATE, DELETE

3. DQL - Data Query Language
   Retrieves data.
   Command: SELECT

4. DCL - Data Control Language
   Controls permissions.
   Commands: GRANT, REVOKE

5. TCL - Transaction Control Language
   Manages transactions.
   Commands: COMMIT, ROLLBACK, SAVEPOINT

--------------------------------------------------
9. PRACTICAL SQL EXERCISE
--------------------------------------------------

STEP 1: CREATE DATABASE

CREATE DATABASE company;

STEP 2: SELECT DATABASE (MYSQL)

USE company;

STEP 3: CREATE EMPLOYEE TABLE

CREATE TABLE employees (
    employee_id INT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    department VARCHAR(50),
    salary DECIMAL(10,2)
);

STEP 4: INSERT RECORDS

INSERT INTO employees
(employee_id, name, age, department, salary)
VALUES
(1, 'Rahul', 23, 'IT', 30000),
(2, 'Priya', 24, 'HR', 35000),
(3, 'Amit', 22, 'Sales', 25000);

STEP 5: DISPLAY RECORDS

SELECT * FROM employees;

EXPECTED OUTPUT:

employee_id | name  | age | department | salary
1           | Rahul | 23  | IT         | 30000
2           | Priya | 24  | HR         | 35000
3           | Amit  | 22  | Sales      | 25000

NOTE:
These database creation commands are written for MySQL. SQLite uses a different database creation workflow.

--------------------------------------------------
10. DAY 1 INTERVIEW QUESTIONS
--------------------------------------------------

Q1. What is SQL?
Ans: SQL is a language used to communicate with databases.

Q2. What is a database?
Ans: A database is an organized collection of data.

Q3. What is DBMS?
Ans: DBMS is software used to manage databases.

Q4. What is RDBMS?
Ans: RDBMS stores data in related tables.

Q5. Difference between DBMS and RDBMS?
Ans: DBMS manages databases, while RDBMS organizes data into related tables.

Q6. What is a table?
Ans: A table stores data in rows and columns.

Q7. What is a row?
Ans: A row represents a single record.

Q8. What is a column?
Ans: A column represents an attribute or field.

Q9. What is a primary key?
Ans: A primary key uniquely identifies each record.

Q10. What is a foreign key?
Ans: A foreign key connects related tables.

Q11. What is NULL?
Ans: NULL represents missing or unknown data.

Q12. What is VARCHAR?
Ans: VARCHAR stores variable-length text.

Q13. Difference between INT and DECIMAL?
Ans: INT stores whole numbers, while DECIMAL stores exact decimal values.

Q14. What is DDL?
Ans: DDL defines database structures.

Q15. What is DML?
Ans: DML modifies database records.

Q16. What is DQL?
Ans: DQL retrieves data from databases.

Q17. What is DCL?
Ans: DCL manages database permissions.

Q18. What is TCL?
Ans: TCL manages database transactions.

Q19. What is CREATE?
Ans: CREATE is used to create database objects.

Q20. What is SELECT?
Ans: SELECT retrieves data from a table.

--------------------------------------------------
11. DAY 1 HOMEWORK
--------------------------------------------------

1. Understand SQL and its purpose.
2. Learn DBMS and RDBMS.
3. Understand tables, rows and columns.
4. Learn primary key and foreign key.
5. Study SQL data types.
6. Understand five categories of SQL commands.
7. Create a company database.
8. Create an employees table.
9. Insert at least 5 employee records.
10. Practice SELECT * query.

--------------------------------------------------
12. GITHUB UPDATE
--------------------------------------------------

File Name:
Day-01-Introduction-to-SQL.txt

Suggested Commit Message:

Day 01: SQL introduction and database fundamentals

Git Commands:

git add .
git commit -m "Day 01: SQL introduction and database fundamentals"
git push

--------------------------------------------------
DAY 1 COMPLETED
--------------------------------------------------

NEXT DAY - DAY 02

Topics:
1. SELECT
2. DISTINCT
3. WHERE
4. ORDER BY
5. LIMIT
6. AND
7. OR
8. NOT

Keep Learning. Keep Practicing. Keep Growing!

MY GOAL:
Become a Professional Data Analyst.
