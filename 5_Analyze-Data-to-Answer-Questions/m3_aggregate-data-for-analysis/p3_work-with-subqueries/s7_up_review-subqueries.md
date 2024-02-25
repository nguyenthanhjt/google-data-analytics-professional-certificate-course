# Review subqueries

## SQL subqueries

Multiple choice exercise

Features of subqueries

A subquery is a SQL query nested inside a larger query. Review a series of statements about subqueries and answer whether they are true or false.

- You can use comparison operators such as >, <, or = within subqueries.

> Comparison operators such as >, <, or = help you compare data in subqueries. You can also use multiple row operators including IN, ANY, or ALL.

- A subquery is also called an outer query or outer select. The statement containing a subquery is called an inner query or inner select.

> The statement containing a subquery is an outer query or outer select. Subqueries are nested within these statements, called inner queries or inner select.

- The parent query executes before its inner query.

> The innermost query executes first. Its parent query executes last so it can use the results returned by inner queries.

- The outer quey is executed before inner queries:

> The innermost query executes first. Its parent query executes last so it can use the results returned by inner queries.

- A subquery can have more than one column specified in the SELECT clause.

> For a subquery to compare multiple columns, those columns must be selected in the main query.

- A subquery can’t be nested in a SET command.

> A SET command can’t have a nested subquery because it is used with UPDATE to adjust specific columns and values in a table.

- Subqueries that return more than one row can only be used with multiple value operators.

> Subqueries that return more than one row rely on multiple value operators such as the IN command.
