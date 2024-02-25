# Practice Quiz - Hands-on activity: Use subqueries

## Activity Overview

As a data analyst, you will sometimes want to analyze a small subset of data that is contained within a much larger dataset. This is when subqueries can be really useful. As you’ve been learning, subqueries are queries that are nested inside of another query. Some queries can have many subqueries, while others may have only one. It’s important to know how subqueries function and to understand the different components you can use to create them.

In this activity, you will work with queries and subqueries to examine a public health dataset. You will create subqueries to discover which industries receive an unusual number of complaints and, more importantly, which industries are connected to serious health issues. This will allow you to allocate your resources more effectively to safeguard public health.

## Scenario

Review the following scenario. Then complete the step-by-step instructions.

In this scenario, you are a junior data analyst for a multinational food and beverage manufacturer. You and your team are responsible for maintaining the safety of a wide array of food products. Because of the overwhelming number of products on the market, you have been asked to prioritize which products need to be reviewed by your stakeholders.

While it's useful to know which food industries receive the most complaints, the more critical aspect to consider is identifying the complaints that lead to severe health consequences, such as hospital visits.

To complete this task, you'll analyze food event reports for targeted health interventions.

## Step by step Instructions

Follow the instructions to complete each step of the activity. Then answer the question at the end of the activity before going to the next course item.

### Step 1: Access the public dataset

1. Log in to BigQuery and open the [BigQuery Console](https://console.cloud.google.com/bigquery).

    *Note: BigQuery frequently updates its user interface. The latest changes may not be reflected in the screenshots presented in this activity, but the principles remain the same. Adapting to changes in software updates is an essential skill for data analysts, and it’s helpful for you to practice troubleshooting. You can also reach out to your community of learners on the discussion forum for help.*

2. Before you can load the `fda_food` dataset, you need to have `bigquery-public-data` pinned in the Explorer menu of your SQL Workspace. Follow these steps to pin the dataset:

   a. Enter `public` in the Explorer menu search box, and press Enter/Return on your keyboard.
   b. Select `SEARCH ALL PROJECTS`.
   c. Scroll to find `bigquery-public-data` and select the star to pin it.

3. Add the FDA food dataset. Follow these steps:

   a. Select the arrow next to the `bigquery-public-data` to expand its contents.
   b. Scroll to find `fda_food`. You may have to select `SHOW MORE` to view the dataset listed.

   ![Explorer search results with the path to the fda_food dataset. The food_enforcement table is selected.](image_url_1)

   c. Expand `fda_food` and select `food_enforcement`.
   d. Select the `Preview` tab in the viewer to examine the table data.

   ![Preview tab is open and displaying the rows in the food_enforcement table.](image_url_2)

4. Next, select the `food_events` table from the `fda_food` dataset, then select `Preview` to examine the table data.

Once you have taken some time to explore the tables within the `fda_food` dataset, you are ready to begin working with subqueries!

### Step 2: Gather an initial overview

To get an initial overview, run a SQL query to identify which food industries have the highest number of complaints. This will provide an initial dataset to work from. To find the top industries for recalls, perform the following steps:

1. Create a new query.

2. Enter the following in the query editor:

    ```sql
    SELECT 
    products_industry_name, 
    COUNT(report_number) AS count_reports
    FROM bigquery-public-data.fda_food.food_events
    GROUP BY products_industry_name
    ORDER BY count_reports DESC
    LIMIT 10;
    ```

    *Note: Depending on the type of web browser you are using, you may have issues conducting a direct copy + paste of the above syntax directly from this assignment to your BigQuery workspace. If you are experiencing this issue, open two separate windows on your screen to manually enter the above information into the BigQuery workspace area.*

3. You have the option to save your query as a table. To do this, select the `MORE` menu from the Query Editor and open the Query Settings menu. In the Query Settings menu, select `Set a destination table for query results`. Set the dataset option to `demos` and name the table `reports_by_industry`.

    *The Query settings menu with a new dataset titled `dac5bigquery.FDA_demos` and table ID titled `reports_by_industry` added.*

4. Select `RUN`. The query will save as a new table in your `demos` dataset.

*The Query results window will populate with a table containing two columns and 10 rows. The first column is `products_industry_name`, and the second is `count_reports`. The 10 different industries are listed in descending order in the rows.*

Take some time to check the different industries and the differences in report numbers. You can modify your search to examine the different symptoms that consumers experienced (reactions) based on products (`products_brand_name`) as well as the outcomes or consequences from each food event.

*The table lists the top ten industries with the highest count of reported complaints.*

### Step 3: Determine the number of hospitalizations

With a list of the industries receiving the most complaints, your next step is to find out which of these complaints led to hospitalizations. Filter the initial list accordingly and focus solely on complaints that resulted in hospital visits.

To find out which industries among the most complained about are associated with hospitalizations, follow these steps:

1. Create a new query.

2. Enter the following into the editor:

    ```sql
    SELECT 
    products_industry_name, 
    COUNT(report_number) AS count_hospitalizations
    FROM
    bigquery-public-data.fda_food.food_events
    WHERE products_industry_name IN
    (SELECT 
        products_industry_name
    FROM 
        bigquery-public-data.fda_food.food_events
    WHERE 
        products_industry_name IS NOT NULL
        AND products_industry_name != ''
        AND outcomes LIKE '%hospitalization%'
    )
    GROUP BY products_industry_name
    ORDER BY count_hospitalizations DESC
    LIMIT 10;
    ```

    The outer query is similar to the previous one. It selects product industry names, counts the number of reports, and labels them as `count_hospitalizations`. The query pulls this data from the `food_events` table.

    The subquery starts with a `WHERE` clause and an `IN` operator, allowing the subquery to specify multiple values. The second `SELECT` statement tells the subquery to pull the product industry names FROM the `food_events` table in the FDA_food dataset. Results are grouped by product industry name and ordered in descending order. `LIMIT` specifies to limit the results to 10. `AND` and `LIKE` are used to indicate if hospitalizations are present within the outcomes field.

    The outer query is then closed by grouping results by `product_industry_name` and ordering in descending order by the number of hospitalizations recorded.

3. You can also save this query as a table. Before running the query, select the `MORE` menu from the Query Editor and open the Query Settings menu. In the Query Settings menu, select `Set a destination table for query results`. Set the dataset option to `demos` and name the table `reports_with_hospitalizations`.

4. Select `RUN`. The query will save as a new table in your `demos` dataset.

*The Query results window will populate with a table containing two columns and ten rows. The first column is `products_industry_name`, and the second is `count_hospitalizations`. The 10 different industries are listed in descending order in the rows.*

Take some time to review the different industries and the differences in reported hospitalizations. You can modify your search to examine the different symptoms that consumers experienced (reactions) based on products (`products_brand_name`); the dates in which the food events occurred (`date_started`); and the outcomes, or consequences, from each food event. These modifications will allow you to find and analyze any links among fields within the datasets for your research.

*The table lists the top ten industries with the highest count of reported hospitalizations.*

Great work! Through this process, you discovered which industries receive an unusual number of complaints and, more importantly, which are connected to serious health issues. This knowledge allows you to allocate your resources more effectively to safeguard public health. By completing this activity, you have created subqueries using SELECT statements with FROM, GROUP BY, WHERE, IN, AS, COUNT, and ORDER BY clauses, as well as AND and LIKE operators to search and analyze the query results relating to reports of food events by industry.

## Reflection

In the text box below, write 2-3 sentences (40-60 words) in response to each of the following questions:

- Why is working with subqueries an important skill for data analysts to learn?
- What are some benefits of using subqueries?

What do you think?
Your answer cannot be more than 10000 characters.

> Correct
>
> Congratulations on completing this hands-on activity! In this activity, you created queries and subqueries to analyze sections of a large dataset. An effective response might include: 
> Learning how to create queries and subqueries is a key component to the ability to research and deliver useful findings to your leadership or businesses.
>
> Subqueries help you identify and work with smaller sections of data from a large dataset.
>
> Subqueries can be challenging—they take practice and repetition to execute well. Now that you have a starting point, take some time to practice working with different datasets within the bigquery-public-data database and building out your own subqueries. 
