# Practice Quiz - Test your knowledge on working with subqueries

## Question 1

1. **Which of the following queries contain subqueries? Select all that apply.**

   - Query 1:

     ```sql
     SELECT product_name,
     CASE
     WHEN price < 10 THEN 'Low price'
     WHEN price >= 10 AND price < 20 THEN 'Medium price'
     ELSE 'High price'
     END AS price_category
     FROM products
     ```

   - `Query 2`:

     ```sql
     SELECT price
     FROM sales
     WHERE price = (SELECT MAX(salary) FROM sales)
     ```

   - Query 3:

     ```sql
     SELECT call
     FROM recordings
     ORDER BY call.employee_id, call.start_time
     ```

   - `Query 4`:

     ```sql
     SELECT employee_id
     FROM employees
     WHERE department_id IN (SELECT department_id FROM departments WHERE location_id = 1000)
     ```

> Query 2 and Query 4 are correct: The two queries with statements in parentheses contain subqueries. A subquery is a SQL query that is nested inside a larger query.

## Question 2: **When working with subqueries, which query will execute first?**

- `Innermost`
- Rightmost
- Outermost
- Leftmost

> When working with subqueries, the innermost query will execute first.

### Question 3: Which HAVING clause indicates to only retrieve products that have been sold more than 100 times?**

- `HAVING COUNT(order_items.product_id) > 100`
- HAVING COUNT(order_items.product_id) < 100
- HAVING (order_items.product_id) > 100
- HAVING (order_items.product_id > 100)

> The HAVING clause HAVING COUNT(order_items.product_id) > 100 indicates to only retrieve products that have been sold more than 100 times.

### Question 4: **Fill in the blank: A data professional uses the SQL _____ statement to return records that meet conditions by including an if/then statement in a query.**

- `CASE`
- HAVING
- WHEN
- CONCAT

> A data professional uses the SQL CASE statement to return records that meet conditions by including an if/then statement in a query.
