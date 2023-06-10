# EXP-01---FETCH---ALIAS-
## AIM:
To write SQL query to fetch "FIRST_NAME" from the worker table using the alias name from the sample data.

## ALGORITHM:

1.Start by connecting to your database.

2.Formulate the SQL query:

3.Begin with the "SELECT" statement.

4.Specify the column you want to retrieve, in this case, "FIRST_NAME".

5.Specify the table from which you want to fetch the data.

6.Execute the SQL query.

7.Fetch the result set returned by the query.

8.Process the result set:

9.Iterate over the rows of the result set.

10.Access the value of the "FIRST_NAME" column for each row.

11.Perform any required operations on the fetched data.

12.Close the database connection.

## PROGRAM:
```
CREATE TABLE Worker (
  WORKER_ID INT NOT NULL PRIMARY KEY,
  FIRST_NAME CHAR(25),
  LAST_NAME CHAR(25),
  SALARY INT(15),
  JOINING_DATE DATETIME,
  DEPARTMENT CHAR(25)
);

INSERT INTO Worker(WORKER_ID, FIRST_NAME, LAST_NAME, SALARY, JOINING_DATE,DEPARTMENT) VALUES
  (001, 'Monika', 'Arora', 100000, '14-02-2009.00.00', 'HR'),
  (002, 'Niharika', 'Verma', 80000, '14-06-1109.00.00', 'Admin'),
  (003, 'Vishal', 'Singhal', 300000, '14-02-2009.00.00', 'HR'),
  (004, 'Amitabh', 'Singh', 500000, '14-02-2009.00.00', 'Admin'),
  (005, 'Vivek', 'Bhati', 500000, '14-06-11 09.00.00','Admin'),
  (006, 'Vipul', 'Diwan', 200000, '14-06-11 09.00.00','Account'),
  (007, 'Satish', 'Kumar', 75000, '14-01-20 09.00.00','Account'),
  (008, 'Geetika', 'Chauhan', 90000, '14-04-1109.00.00', 'Admin');

SELECT FIRST_NAME AS WORKER_NAME from Worker;
```
## OUTPUT:
![image](https://github.com/swethamohanraj/EXP-01---FETCH---ALIAS-/assets/94228215/e6e1ed47-3e56-46e0-b18f-08383d95298f)

## RESULT:
Thus a SQL query is created to fetch data from table using alias name.
