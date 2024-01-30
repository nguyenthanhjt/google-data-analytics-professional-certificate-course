# Practice Quiz: Test your knowledge on sorting data with SQL

## Question 1: A data analyst at a gift retailer sorts a list of handmade candles by price from least expensive to most expensive. Which statement do they use?

- `ORDER BY candle_price`
- ORDER BY candle_price DESC
- WHERE candle_price
- WHERE candle_price ASC

> They use ORDER BY candle_price. An ORDER BY statement sorts in ascending order by default. ORDER BY column_title is the syntax for this query.

## Question 2:What will this query return?

```sql
SELECT *
FROM widgets
WHERE
ORDER BY 
    manufacture_date DESC
```

- All of the columns in the manufacture_date table
- `All of the rows in the widgets table, with the most-recently manufactured widgets listed first`
- All of the rows in the widgets table, with the least-recently manufactured widgets listed first
- All of the rows in the widgets table

> The query will return all of the rows in the widgets table, ordered by the manufacture_date column in descending order. This means the most recently manufactured widgets will be returned first.

## Question 3: You are working with a database table that contains employee data. Which ORDER BY clause will sort employees by the earliest hire dates at the top of the list?

- ORDER BY hire_date DESC
- ORDER BY hire_date REV
- ORDER BY hire_date MIN
- `ORDER BY hire_date ASC`

## Question 4:What SQL operator enables a data professional to filter for two conditions at once when using a WHERE statement?

- IN
- Plus sign +
- `AND`
- Ampersand &

> The AND operator enables a data professional to filter for two conditions at once when using a WHERE statement.
