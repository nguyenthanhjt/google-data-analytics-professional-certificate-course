# Practice Quiz - Hands-On Activity: Use subqueries to refine data

## Activity Overview

As you’ve learned, a subquery is a query that is nested inside of another query. The subquery filters or sorts data to prepare it to be used by the outer query to produce its final result. This allows data professionals to create more nuanced queries that provide specific insights from the data!

For example, perhaps a data analyst working in human resources has been asked to determine the average salary of employees working within a specific department. The analyst can use a subquery to first find the total salary and number of employees within the department. Then, the outer query will use these numbers to calculate the average salary within a department. It's a step-by-step process, each step relying on the one before it.

In this activity, you will practice using SELECT statements with FROM, WHERE, and GROUP BY clauses to build your subqueries. By the time you complete this activity, you will be able to create a subquery using SELECT statements with FROM, WHERE, and GROUP BY clauses and analyze the query’s results.

## Scenario

Review the following scenario. Then complete the step-by-step instructions.

You work for an organization that is responsible for the safety, efficiency, and maintenance of transportation systems in your city. You have been asked to gather information around the use of Citi Bikes in New York City. This information will be used to convince the mayor and other city officials to invest in a bike sharing and rental system to help push the city toward its environmental and sustainability goals.

To complete this task, you will create three different subqueries, which will allow you to gather information about the average trip duration by station, compare trip duration by station, and determine the five stations with the longest mean trip durations.

## Step-By-Step Instructions

### Step 1: Access the dataset

For this activity, you will need to log in to your BigQuery account to use the public new_york_citibike dataset. Then, use the table called citibike_trips. For a refresher on how to access this data, refer to the optional reading Prepare to use the bike sharing dataset in BigQuery.

### Step 2: Create a subquery to find the average trip duration by station

1. Select COMPOSE A NEW QUERY from the SQL workspace in BigQuery. Or, if you have the new_york_citibike.citibike_trips table open, select Query from the table's menu to compose a new query.

2. In line 1, enter SELECT, then press Enter/Return.

3. In line 2, press Tab, then enter subquery.start_station_id followed by a comma. Then press Enter/Return.

4. In line 3, enter subquery.avg_duration, then press Enter/Return.

     1–3 in the query should read as follows:

    ```sql
    SELECT
        subquery.start_station_id,
        subquery.avg_duration
    ```

    This SELECT statement is used to create the outer query. The fields identified in lines 2 and 3 allow the SELECT statement to function similarly to a table with an alias, e.g. SELECT alias.column_name1, alias.column_name2. This relies on the subquery below to populate the Query results table.

5. In line 4, press Backspace to remove the indentation to align the text with the SELECT statement. Enter FROM, then press Enter/Return.

6. In line 5, press Tab, then enter an open parenthesis [(]. Then press Enter/Return.

7. In line 6, press Tab, then enter SELECT. Then press Enter/Return.

8. In line 7, press Tab, then enter start_station_id followed by a comma. Then press Enter/Return.

9. In line 8, enter AVG(tripduration) as avg_duration. Then press Enter/Return.

    Lines 4–8 in the query should read as follows:

    ```sql
    FROM
        (
        SELECT
            start_station_id,
            AVG(tripduration) AS avg_duration
    ```

    The subquery is created by using another SELECT statement, located within a FROM clause. It is used to determine the average trip duration by station. The station is indicated by the start_station_id. The average is calculated using the AVG function and is given the alias avg_duration using AS. This will appear as a column title in the results table after you run the query.

10. In line 9, press Backspace to remove the indentation to align the text with the SELECT statement.

11. Still in line 9, enter FROM bigquery-public-data.new_york_citibike.citibike_trips, then press Enter/Return.

12. In line 10, enter GROUP BY start_station_id) as subquery; Notice that this line closes the parentheses that opened in line 2.

13. In line 11, add ORDER BY avg_duration DESC;.

    Lines 9, 10, and 11 in the query should read as follows:

    ```sql
    FROM bigquery-public-data.new_york_citibike.citibike_trips
    GROUP BY start_station_id) as subquery
    ORDER BY avg_duration DESC;
    ```

    FROM will tell the subquery where to pull the data from. In this case, it’s pulling from the citibike_trips table. GROUP BY will group the rows by columns. Notice how it has the alias, subquery. This is what links to the two fields designated to be the titles of the results columns, as indicated in the outer query.

    The complete query should read as follows:

    ```sql
    SELECT
        subquery.start_station_id,
        subquery.avg_duration
    FROM
        (
        SELECT
            start_station_id,
            AVG(tripduration) as avg_duration
        FROM bigquery-public-data.new_york_citibike.citibike_trips
        GROUP BY start_station_id) as subquery
    ```

14. Select RUN. The results will appear in the Query results window.

Note: Your results should contain two columns: start_station_id and avg_duration, however, the specific rows may differ from what is depicted here due to periodic refreshes of the source tables on BigQuery.

The Query results window showing the first 13 (of 882) rows of results. Column names are start_station_id and avg_duration.
Take some time to examine the query results. In this case, there are 882 lines of data that you can use to analyze and compare the average trip durations between each station. You will continue to work with the average trip duration per station in the next query.

### Step 3: Create a subquery to compare trip duration by station

1. Select the blue plus sign tab to compose a new query.
2. Enter the following query:

    ```sql
    SELECT
        starttime,
        start_station_id,
        tripduration,
        (
            SELECT ROUND(AVG(tripduration),2)
            FROM bigquery-public-data.new_york_citibike.citibike_trips
            WHERE start_station_id = outer_trips.start_station_id
        ) AS avg_duration_for_station,
        ROUND(tripduration - (
            SELECT AVG(tripduration)
            FROM bigquery-public-data.new_york_citibike.citibike_trips
            WHERE start_station_id = outer_trips.start_station_id
        ), 2) AS difference_from_avg
    FROM bigquery-public-data.new_york_citibike.citibike_trips AS outer_trips
    ORDER BY difference_from_avg DESC
    LIMIT 25;
    ```

3. Select RUN. The results will appear in the Query results window.

### Step 4: Create a subquery to determine the five stations with the longest mean trip duration

1. Enter the following query:

    ```sql
    SELECT
        tripduration,
        start_station_id
    FROM bigquery-public-data.new_york_citibike.citibike_trips
    WHERE start_station_id IN
        (
            SELECT
                start_station_id
            FROM
            (
                SELECT
                    start_station_id
                FROM bigquery-public-data.new_york_citibike.citibike_trips
                GROUP BY start_station_id
                ORDER BY AVG(tripduration) DESC
                LIMIT 5
            ) AS top_five
        );
    ```

2. Select RUN. The results will appear in the Query results window.

## Reflection

### Question 1

The last query you ran returned every record from only the top five stations with the highest average trip durations. How would you modify the previous query to find all the records from the five stations with the lowest average trip durations?

- `Change DESC to ASC in line 17` - Correct
- Change AVG(tripduration) AS avg_duration to MIN(tripduration) AS min_duration in line 13
- Change top_five to bottom_five in line 16
- Change 5 to -5 in line 18

### Question 2

In the text box below, write 2-3 sentences (40-60 words) in response to each of the following questions:

**How do subqueries help you work with large datasets?**

Subqueries allow you to break down complex tasks into smaller, manageable steps. By using subqueries, you can filter, aggregate, or manipulate data before incorporating it into the main query, making it more efficient and focused. This is particularly beneficial when dealing with large datasets, as it optimizes the query performance.

**Which other ways could you use subqueries to analyze data?**

Subqueries can be used for various analytical purposes, such as calculating percentages, identifying outliers, or comparing trends over time. They are valuable for tasks like finding correlations, filtering data based on specific conditions, or performing calculations on aggregated results. Additionally, subqueries enable the analysis of relationships between different subsets of data, providing a versatile tool for in-depth data exploration.

> In this activity, you created queries and subqueries to compare and analyze specific sections of a large dataset. Effective responses to the reflection questions might include:
>
> - Learning how to create queries and subqueries is a key component of an analyst’s ability to research and deliver useful findings to leadership or team members.
> - Subqueries help you identify and work with smaller sections of data from a large dataset.
> - Subqueries can be used to complete multiple operations at one time rather than creating multiple queries.  They can be used to compare, sort, order, group, and aggregate, among many others.
>
> Subqueries can be challenging—they take practice and repetition to execute well. Now that you have a starting point, take some time to practice working with different datasets within the bigquery-public-data database and building out your own subqueries.
