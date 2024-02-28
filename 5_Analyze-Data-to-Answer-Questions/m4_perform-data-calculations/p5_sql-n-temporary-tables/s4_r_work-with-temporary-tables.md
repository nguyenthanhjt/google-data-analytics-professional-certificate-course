# Work with Temporary Tables

**Temporary tables** are tables in a SQL database that are not stored permanently. In this reading, you will learn methods to create temporary tables using SQL commands and best practices when working with them.

## Quick Refresher on Temporary Tables

- **Automatically Deleted:** Temporary tables are deleted from the database when you end your SQL session.
- **Holding Area:** They can store values as a holding area for series of calculations (pre-processing of data).
- **Data Staging:** Used to collect results of multiple, separate queries, facilitating further analysis.
- **Filtered Subset:** Can store a filtered subset of the database, reducing the need to select and filter data each time.

It is important to point out that each database has its own unique set of commands to create and manage temporary tables. We have been working with BigQuery, so we will focus on the commands that work well in that environment. The rest of this reading will go over the ways to create temporary tables, primarily in BigQuery.

## Working with BigQuery

Each database has its own commands to manage temporary tables. For BigQuery, focus will be on its commands.

### Temporary Table Creation in BigQuery

Temporary tables can be created using the `WITH` clause. The general syntax is as follows:

```sql
WITH
new_table_data AS (
  SELECT *
  FROM Existing_table
  WHERE Tripduration >= 60
)
```

- Begins with the `WITH` clause, followed by the new temporary table name.
- Uses `AS` clause to put data from a `SELECT` statement into the new table.
- Subquery in parentheses filters data from an existing table.

When the database executes this query, it will first complete the subquery and assign the values that result from that subquery to `new_table_data`, which is the temporary table. You can then run multiple queries on this filtered data without having to filter the data every time.

### Temporary Table Creation in Other Databases

While not supported in BigQuery, other databases use `SELECT` and `INTO` to create temporary tables. Syntax:

```sql
SELECT
*
INTO
AfricaSales
FROM
GlobalSales
WHERE
Region = "Africa"
```

- Uses `INTO` clause to store requested data in a new temporary table.

### User-Managed Temporary Table Creation

Analysts can create and manage their temporary tables using the `CREATE TABLE` statement:

```sql
CREATE TABLE table_name (
  column1 datatype,
  column2 datatype,
  column3 datatype,
  ...
)
```

After use, remove the table from the database using `DROP TABLE`:

```sql
DROP TABLE table_name
```

Note: BigQuery uses `CREATE TEMP TABLE` instead of `CREATE TABLE`.

## Best Practices

- **Global vs. Local Temporary Tables:** Local tables are likely used; dropped after the user's session. Global tables are available to all users.
- **Dropping After Use:** Dropping a table removes both data and table variable definitions. Good practice for database performance.

## For More Information

- [BigQuery Documentation for Temporary Tables](https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#temporary_tables): Syntax for creating temporary tables in BigQuery.
- [How to use Temporary Tables via WITH in Google BigQuery](https://www.pascallandau.com/bigquery-snippets/use-temporary-tables-with-named-subquery/?utm_source=blog&utm_medium=rss&utm_campaign=development-**feed**): Describes how to use `WITH` clause.
- [Introduction to Temporary Tables in SQL Server](https://codingsight.com/introduction-to-temporary-tables-in-sql-server/): Describes `SELECT INTO` and `CREATE TABLE`.
- [SQL Server Temporary Tables](https://www.sqlservertutorial.net/sql-server-basics/sql-server-temporary-tables/): Details on temporary table creation and removal.
- [Choosing Between Table Variables and Temporary Tables](https://www.red-gate.com/hub/product-learning/sql-prompt/choosing-table-variables-temporary-tables): Differences between passing variables and using temporary tables.
