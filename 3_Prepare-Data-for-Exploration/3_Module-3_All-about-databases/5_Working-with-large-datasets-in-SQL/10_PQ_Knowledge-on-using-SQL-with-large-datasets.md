# Test your knowledge on using SQL with large datasets

## Question 1: In MySQL, what is acceptable syntax for the SELECT keyword? Select all that apply

- `SELECT`
- `select`
- "SELECT"
- 'SELECT'

> n MySQL, SELECT or select is acceptable syntax.

## Question 2:A database table is named blueFlowers. What type of case is this?

- Lowercase
- `Camel case`
- Snake case
- Sentence case

>blueFlowers is in camel case.

## Question 3:In BigQuery, what optional syntax can be removed from the following FROM clause without stopping the query from running?

FROM `bigquery-public-data.sunroof_solar.solar_potential_by_postal_code`

- Dashes
- Underscores
- Dots
- `Backticks`

>The name of the dataset is shown between two backticks to help people read the query more easily. If you remove the backticks, the query will still run.

## Question 4:In the following FROM clause, what is the table name in the SQL query?

`FROM bigquery-public-data.sunroof_solar.solar_potential_by_postal_code`

- `solar_potential_by_postal_code`
- sunroof_solar
- public-data.sunroof
- solar.solar

> The table name in the SQL query is solar_potential_by_postal_code. This table is in the sunroof_solar dataset, a public dataset in BigQuery.
