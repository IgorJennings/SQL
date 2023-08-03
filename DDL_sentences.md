
# DDL Sentences
## Data Defenition Languages

### Create table
```SQL
CREATE TABLE IF NOT EXIST
```

--CRETING TABLES
CREATE TABLE IF NOT EXIST name of table(
    variable_1,
    variable_2,
    variable_3,
    variable_n
);

Example:
CREATE TABLE IF NOT EXIST employees(
    id_employees INT
);

Look all elements of a table:
SELECT * FROM table name;

Example:
SELECT * FROM employees;

--Type of data: BOOLEAN
CREATE TABLE IF NOT EXIST employees(
    id_employees INT,
    married BOOLEAN
);


--ADDING COLUMS TO THE TABLES

--INSERT DATA:
INSERT INTO table name (colum_1,column_2,...,column_n) VALUES (value_for_column_1,value_for_column_2,...,value_for_column_n);

Example:
INSERT INTO employees (id_employees,married) VALUES (1,TRUE);
INSERT INTO employees (id_employees,married) VALUES (2,FALSE);


--TYPE OF DATA: TEXT, CHAR, VARCHAR
EXAMPLE:
CREATE TABLE IF NOT EXIST employees(
    id_employees INT,
    married BOOLEAN,
    name VARCHAR(250),
    genre CHAR(1)
);


--DELETING TABLES
DROP TABLE IF EXISTS name of the table;

Example:
DROP TABLE IF EXISTS employees;



