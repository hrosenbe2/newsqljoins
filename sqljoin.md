# # SQL Joins

## Learning Objectives.
- Define SQL joins.
- Explain what SQL joins and how to use them.
- Use the different type of joins to display records.
- Shopping datbase example

## Opening Framing (5 / 5)
An SQL JOIN clause is used to combine rows from two or more tables, based on a common field between them.

The most common type of join is: SQL INNER JOIN (simple join). An SQL INNER JOIN returns all rows from multiple tables where the join condition is met.

### Information Dive (5 / 10)
For the next 5 minutes, research SQL joins are

[SQL Joins](http://www.w3schools.com/sql/sql_join.asp)

### T&T (5 / 15)
Now, turn & talk to your neighbor and discuss:

1. At a high level, what are sql joins and how might they be useful?
2. How many differnt join statements are there?




## Different SQL JOINs
Before we continue with examples, we will list the types of the different SQL JOINs you can use:

- INNER JOIN: Returns all rows when there is at least one match in BOTH tables

- LEFT JOIN: Return all rows from the left table, and the matched rows from the right table
- RIGHT JOIN: Return all rows from the right table, and the matched rows from the left table
- FULL JOIN: Return all rows when there is a match in ONE of the tables

## SQL INNER JOIN Keyword
The INNER JOIN keyword selects all rows from both tables as long as there is a match between the columns in both tables.

## SQL INNER JOIN Syntax

```
SELECT column_name(s)
FROM table1
INNER JOIN table2
ON table1.column_name=table2.column_name;
```

![Inner JOIN](https://github.com/ATL-WDI-Curriculum/sql-joins/blob/master/images/img_innerjoin.gif)

## SQL LEFT JOIN Keyword

The LEFT JOIN keyword returns all rows from the left table (table1), with the matching rows in the right table (table2).
The result is NULL in the right side when there is no match.

```
SELECT column_name(s)
FROM table1
LEFT JOIN table2
ON table1.column_name=table2.column_name;
```

![Left JOIN](http://www.w3schools.com/sql/img_leftjoin.gif)
![example](https://github.com/ATL-WDI-Curriculum/newsqljoins/blob/master/images/sqlleft.png)
[sql join left](http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_join_left)


## SQL RIGHT JOIN Keyword
The RIGHT JOIN keyword returns all rows from the right table (table2), with the matching rows in the left table (table1). The result is NULL in the left side when there is no match.

SQL RIGHT JOIN Syntax

```
SELECT column_name(s)
FROM table1
RIGHT JOIN table2
ON table1.column_name=table2.column_name;
```

![right](https://github.com/ATL-WDI-Curriculum/newsqljoins/blob/master/images/img_rightjoin.gif)

![example](https://github.com/ATL-WDI-Curriculum/newsqljoins/blob/master/sqljoinright.png)

[sql join right](http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_join_right&ss=-1)

## SQL FULL OUTER JOIN Keyword

The FULL OUTER JOIN keyword returns all rows from the left table (table1) and from the right table (table2).
The FULL OUTER JOIN keyword combines the result of both LEFT and RIGHT joins.
The FULL OUTER JOIN keyword returns all the rows from the left table (Customers), and all the rows from the right table (Orders). If there are rows in "Customers" that do not have matches in "Orders", or if there are rows in "Orders" that do not have matches in "Customers", those rows will be listed as well.

SQL FULL OUTER JOIN Syntax

```
SELECT column_name(s)
FROM table1
FULL OUTER JOIN table2
ON table1.column_name=table2.column_name;
```

### Diagram
![full outter](http://www.w3schools.com/sql/img_fulljoin.gif)

### output

![full outter](https://github.com/ATL-WDI-Curriculum/newsqljoins/blob/master/sqlfullouterjoin.png)

### example:

![example](https://github.com/ATL-WDI-Curriculum/newsqljoins/blob/master/sqljoinright.png)
