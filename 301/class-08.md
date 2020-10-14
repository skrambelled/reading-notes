# SQL

Server Query Language

You can use SQL to collect data from databases.

A db is a collection of tables, each with their own cols and rows.

In SQL you can `SELECT` a col `FROM` a table, `WHERE` a conditions is met.

Capitalization is a common convention, but not technically required.

Select all movies:

```sql
SELECT * FROM movies;
```

```sql
-- select multiple cols by separating by commas
SELECT title,director FROM movies

--  select things conditionally (and)
SELECT title FROM movies
WHERE year>=2000 AND year<2010

-- more conditions (or)
SELECT * FROM movies
WHERE year < 2000 OR year > 2010;

```

## SQL operators

* `=` - case sensitive string comparison
* `!=` - case sensitive string comparison
* `LIKE` - case insensitive
* `NOT LIKE` - case insensitive
* `%` - match a sequence of chars (used in conjunction with `LIKE` and `NOT LIKE`)
* `_` - used to match a single character (`LIKE` and `NOT LIKE`)
* `IN("A", "B", "C")` - match a string in a list
* `NOT IN(...)`
* `DISTINCT` - discard duplicates
* `ORDER BY <col> [ASC/DESC]` - sort by a col [optionally in ascending or descending order]
* `LIMIT <num>` - only return num entries
* `OFFSET <num>` - start looking after num entries

## Multiple table queries, using `JOIN`

```SQL
SELECT col1, col2, ...
FROM table1
  JOIN table2
    ON table1.commonCol = table2.commonCol
```

* `INNER JOIN` - when two tables share a common col
* `LEFT JOIN` - keep left tables data even if rigth table is missing it
* `RIGHT JOIN` - keep right, when left is missing
* `FULL JOIN` - keep both, even if either is missing data

## NULL

You should avoid using NULL as an entry in a table, and instead use an appropriate value instead, like 0 or an empty string. Sometimes this is not appropriate, or possible though.

It would not be appropriate to use 0 in a set of numbers if it messes up the average of that set. It is not possible to use an empty string when join tables that don't have matching data sets. Etc.

[<-- Back](../README.md)
