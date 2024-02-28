# Practice Quiz: Test your knowledge on using SQL with temporary tables

## **Question 1:** When working with a temporary table in a SQL database, at what point will the table be automatically deleted?

- `After ending the session in the SQL database`
- After completing all calculations in the table
- After running a report from the table
- After running the query in the SQL database

> Correct:The temporary table will be automatically deleted after ending the session in the SQL database.

## **Question 2:**What data will appear in the temporary table created through this query?

```sql
WITH plant_variety AS (
    SELECT *
    FROM bigquery-public-data.plants.African_species
    WHERE daily_growth_rate_percentage = 0.05
)
```

- All plant species that exist in the public dataset
- Plant varieties that are equal to 0.05 inches tall
- `Plant varieties that grow exactly 0.05 percent per day`
- A random subset of African plant species

> Correct: The temporary table will contain plant varieties that grow exactly 0.05 percent per day. The name of the temporary table is plant_variety and the query includes the condition that the growth rate equals 0.05 percent per day.

## **Question 3:**Fill in the blank: A data analyst uses _____ to copy data from one table into a temporary table without adding the new table to the database

1. COPY TO
2. WITH
3. TEMP
4. `SELECT INTO`

> Correct:A data analyst uses SELECT INTO to copy data from one table into a temporary table without adding the new table to the database. This is useful for making a copy of a table with a specific condition.

## **Question 4:**Why might a data professional add a CREATE TABLE statement to a temporary table?

- Automate calculations in the table
- Give multiple people access to the table
- Include metadata about the data in the table
- Create a second table within the temporary table

> Correct: A data professional might add a CREATE TABLE statement to a temporary table to give multiple people access.
