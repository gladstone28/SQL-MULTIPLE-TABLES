link to lesson:
https://www.codecademy.com/courses/learn-sql-multiple-tables/lessons/multiple-tables/exercises/inner-join-ii


MULTIPLE TABLES
Inner Joins

Let’s revisit how we joined orders and customers. For every possible value of customer_id in orders, there was a corresponding row of customers with the same customer_id.

What if that wasn’t true?

For instance, imagine that our customers table was out of date, and was missing any information on customer 11. If that customer had an order in orders, what would happen when we joined the tables?

When we perform a simple JOIN (often called an inner join) our result only includes rows that match our ON condition.

Consider the following animation, which illustrates an inner join of two tables on table1.c2 = table2.c2:

![](./inner-join.webp)


The first and last rows have matching values of c2. The middle rows do not match. The final result has all values from the first and last rows but does not include the non-matching middle row.


### Instructions
Checkpoint 1 Passed
1.Suppose we are working for The Codecademy Times, a newspaper with two types of subscriptions:

- print newspaper
- online articles

Some users subscribe to just the newspaper, some subscribe to just the online edition, and some subscribe to both.

There is a newspaper table that contains information about the newspaper subscribers.

Count the number of subscribers who get a print newspaper using COUNT().

Use COUNT(*) to count all rows of a table:

```sqlite
SELECT COUNT(*)
FROM newspaper;
```
