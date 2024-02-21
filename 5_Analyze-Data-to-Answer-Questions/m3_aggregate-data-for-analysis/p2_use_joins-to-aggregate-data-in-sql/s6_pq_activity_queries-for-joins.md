# Practice Quiz - Hands-On Activity: Queries for JOINS

## Activity Overview

### Step 1: Load the dataset

1. **Log in to BigQuery Sandbox:**
   Access BigQuery or use the free trial version. On the BigQuery page, click the "Go to BigQuery" button.

2. **Explorer Interface:**
   Navigate to the Editor interface, consisting of the BigQuery navigation menu, Explorer pane, and details pane.

   ![Screenshot of the Explorer pane](#)

3. **Add Public Datasets:**
   Click + ADD in the Explorer pane, then choose Public Datasets. Search for "international education" and select the World Bank's International Education dataset.

   ![Screenshot of the Public Datasets option](#)

4. **View Dataset:**
   Open the dataset in a new tab by selecting the View Dataset button.

5. **Explore Tables:**
   In the Explorer pane, search for `world_bank_intl_education`. Expand the dataset and click SHOW MORE to view additional tables.

   ![Screenshot of the Explorer pane with search](#)

### Step 2: Identify and understand keys

**Understanding JOINs:**
Consider the tables `international_education` and `country_summary`. Identify common columns like 'country_code' for joining. Check table schemas and confirm the shared field.

### Step 3: Review JOINS

**JOIN Types:**
Review various JOIN statements – INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL OUTER JOIN. Understand the implications of each type using Venn diagrams.

### Step 4: Query the dataset and incorporate aliases

**JOIN Example:**
Write a basic JOIN query without aliasing:

```sql
SELECT `bigquery-public-data.world_bank_intl_education.international_education`.country_name,
    `bigquery-public-data.world_bank_intl_education.country_summary`.country_code,
    `bigquery-public-data.world_bank_intl_education.international_education`.value
FROM `bigquery-public-data.world_bank_intl_education.international_education`
INNER JOIN `bigquery-public-data.world_bank_intl_education.country_summary`
ON `bigquery-public-data.world_bank_intl_education.country_summary`.country_code = `bigquery-public-data.world_bank_intl_education.international_education`.country_code
```

### Step 5: Use a JOIN to answer a question

**Query for 2015 Population:**
Write a query to find the 2015 population of the official age for secondary education broken down by region:

```sql
SELECT
    summary.region,
    SUM(edu.value) secondary_edu_population
FROM
    `bigquery-public-data.world_bank_intl_education.international_education` AS edu
INNER JOIN
    `bigquery-public-data.world_bank_intl_education.country_summary` AS summary
ON edu.country_code = summary.country_code
WHERE
    summary.region IS NOT NULL
    AND edu.indicator_name = 'Population of the official age for secondary education, both sexes (number)'
```

### Step 6: Decide when to use INNER JOIN versus OUTER JOINS

**LEFT JOIN Example:**
Write a LEFT JOIN query for NCAA basketball statistics in the 1990s:

```sql
SELECT
 seasons.market AS university,
 seasons.name AS team_name,
 mascots.mascot AS team_mascot,
 AVG(seasons.wins) AS avg_wins,
 AVG(seasons.losses) AS avg_losses,
 AVG(seasons.ties) AS avg_ties
FROM `bigquery-public-data.ncaa_basketball.mbb_historical_teams_seasons` AS seasons
LEFT JOIN `bigquery-public-data.ncaa_basketball.mascots` AS mascots
ON seasons.team_id = mascots.id
```

### Reflection Questions

1. Question 1:   If the last query used an INNER JOIN instead of a LEFT JOIN, it would return - 

- `317`
- 281
- 274
- 324

> The query would return 317 rows. The row count drops from 320 with the LEFT JOIN to 317 with the INNER JOIN, because there are three rows where the team mascot is null. The INNER JOIN drops those rows which is why there is a difference between the two joins in this application.

1. **Reflection:**
   - *Why JOIN Statements Are Important:*
     JOIN statements are crucial for merging data from multiple tables based on common keys, enabling comprehensive analysis.
   - *Consequences of Wrong JOIN Type:*
     Choosing the wrong JOIN type can lead to inaccurate results or missing data, impacting query reliability.
   - *Usefulness of Aliasing:*
     Aliasing is most useful for complex queries, improving readability and maintaining clean, easy-to-understand queries.

> Congratulations on completing this hands-on activity! A thoughtful response would include that JOIN allows you to combine data from linked tables, helping you make comparisons and answer business questions. You might also mention that aliasing helps organize your SQL statements into a structure that is easier to read and follow.
>
> Mastering JOIN statements is one of the most important parts of SQL, as combining data from multiple database tables is a core skill for data analysts.
