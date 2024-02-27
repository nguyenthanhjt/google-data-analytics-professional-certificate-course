# Practice Quiz - Hands-On Activity: From spreadsheets to BigQuery

## Activity Overview

By now, you have worked with data using both spreadsheets and SQL. These tools operate very differently. In spreadsheets, you are able to observe and interact with data directly; with SQL, you interact with data through queries to the database. However, these tools also share a lot of the same functions. And they can even be used together on a project at different stages. In this activity, you’ll be presented with a business scenario where you will need to use a combination of spreadsheets and SQL to clean data, interact with a dataset using SQL, and export results into a new spreadsheet.  

By the time you complete this activity, you will be able to combine tools to successfully analyze data. Switching between spreadsheets and SQL can be challenging because they’re so different, but being able to use them together can streamline your tasks as a data professional. Understanding how to use a given tool and when to use it will be critical when approaching larger and more complex projects in your career as a data analyst.

## Scenario

Review the following scenario. Then complete the step-by-step instructions.

In this scenario, you are working as a data analyst for a national store chain. Management is interested in the amount of inventory being kept in storage at regional sites. Your supervisor has asked you to perform an analysis on inventory and sales data to make recommendations for changes to inventory management practices. You have been provided with three datasets containing information about inventory, products, and sales.

Before you upload these files to BigQuery, you'import them into a spreadsheet to get comfortable with the data and do an initial round of cleaning. To prepare them, you’ll import, inspect, and update the data so it’s useful once you upload it to your database.

These steps may not always be possible to conduct with spreadsheets when working with larger datasets you encounter in the future, but this use case allows you to explore which can be a helpful learning opportunity!

## Step by steps Instructions

Follow the instructions to complete each step of the activity. Then answer the questions at the end of the activity before going to the next course item.

### Step 1: Access the template

To get started, download the three store data .csv files: inventory, products, and sales.

To use the template for this course item, click the link below and select Use Template.

Link to data: [inventory](https://drive.google.com/u/0/uc?id=1FCo85-_jwlOkqucuiizlP3WyCEu1uXBH&export=download), [sales](https://drive.google.com/u/0/uc?id=1hQ3_EqXPANEPhyY-VDKa9LTuB73E_DVT&export=download), and [products](https://drive.google.com/u/0/uc?id=1Qm1FFskt30Cc1I8XbptukBnT3T1ZHeJ-&export=download).

OR

- [inventory.csv](resources/inventory.csv)
- [products.csv](resources/products.csv)
- [sales.csv](resources/sales.csv)

If you don’t have a Google account, download the template directly from the attachment below.

### Step 2: Import the data into a spreadsheet

If you’re using Google Sheets, import the data files into your spreadsheet.

1. Open Sheets.

2. Navigate to the File menu.

3. Select Import from the dropdown list.
    Screenshot of the File menu
4. Select the first file and upload it to the spreadsheet.

5. Choose Replace spreadsheet to insert it into the current sheet.
    Screenshot of the Import file menu
6. Return to the Import menu under the File menu and upload the next file. This time, however, select Insert new sheet(s) to create new worksheet tabs with this file.

7. Repeat these steps until you have all three files added to your spreadsheet.

### Step 3: Inspect the data in the spreadsheet

Applying filters in spreadsheets is an effective way to identify any data that needs to be cleaned. Start by inspecting the Inventory sheet.

1. Navigate to the Inventory sheet.

2. Select any non-blank cell.

3. Open the Data dropdown menu and select Create a filter.

     of the Data dropdown
4. Now you can select the filter icons for each column to inspect the values. Start with the StoreID column. As you scroll through, you might notice that there do not appear to be any blanks or incorrectly entered values. However, if you inspect the StoreName column, you’ll find a blank.

5. Deselect all of the values except for the blank.

6. Select the StoreName filter dropdown

7. Select Clear.

8. Select the checkbox next to the (Blanks) value in the list.

9. Select OK.

    Screenshot of the StoreName filter dropdown
    This should return one row with a missing entry under the StoreName column.

    Screenshot of the missing entry under the StoreName column
    You might be able to find what the missing value is and input it correctly using the filter!

10. Clear the Storename filter and use the StoreId column filter for other stores with the ID 21791.

11. Copy the StoreID (21791)

12. Clear the StoreName Filter using the StoreName filter dropdown. Select Select All then OK.

13. Select the StoreId filter dropdown.

14. Select Clear.

15. Enter 21791 to the search bar which will pull up that StoreID.

16. Select the checkbox next to the 21791 value in the list

17. Select OK.

    Screenshot of the StoreID column with 21791 in each row

### Step 4: Update the data in the spreadsheet

Now that you have checked out your data in a spreadsheet that lets you observe and update your data directly, it’s time to transition to BigQuery so that you can interact with your data using SQL. As you’ve learned, SQL is used to fetch results from queries. While you can also use SQL to clean and update data, that is more commonly managed by database administrators or data engineers. For your purposes, SQL is very powerful when working with larger datasets, especially data in databases! In order to use SQL to query this data, you’ll need to import the data, explore it in your database, and then export the results.

Similar to previous activities, you will need to create a dataset and custom table to house this data before you can inspect it in BigQuery.

1. From the Explorer pane in your BigQuery console, select the three vertical dots next to your project space and select Create dataset.

2. Name the new dataset sales and leave the other settings as their default. Use these settings:

    a. Under Location type, select Multi-Region, then select US (multiple regions in the United States).

    b. Under Advanced options, select Google-managed encryption key for Encryption.

3. Once settings have been verified, select CREATE DATASET.

    Screenshot of the Create dataset window
4. Open the new dataset (sales) info window by selecting the sales item under your project name. Find the row of tab commands.

    Screenshot of the sales dataset window
5. From the sales dataset in your project, select CREATE TABLE.

6. Use the following settings to create your table:

    a. Use the dropdown to set the Create table field to from = UPLOAD.
    b. Select file = Sales.csv from your computer.
    c. Set Table to sales_info
    d. Select the checkbox under Schema for Auto detect.
    e. Leave the default options on all for remaining options.
    f. Select CREATE TABLE.

    Screenshot of the Create table window completed per the instructions

### Step 5: Explore the data in BigQuery

While you did your initial exploration of your datasets in a spreadsheet format, you’re going to continue inspecting your data using BigQuery with SQL. The goal in this section will be to gauge how much of the data will be useful for your analysis and work on putting it together in a useful way. If you haven’t already cleaned the data, exploring it now can be an opportunity to identify various ways to prepare it for analysis.

1. In the Explorer pane, select on the new table: sales_info.

2. Navigate through the SCHEMA and PREVIEW tabs.

    Screenshot of the sales_info table window
3. Open a new QUERY tab.

4. Run the following query (placing your project name in the FROM statement):

    ```sql
    SELECT
    *
    FROM [your_project_name_here].sales.sales_info
    LIMIT 50
    ```

    Your results will return something like this:

    Screenshot of the Query results screen
    You’ve successfully run your first query! Now, check what kind of range of data you have in your dataset. Use MIN and MAX SQL functions to get the oldest and most recent dates with the following query:

    ```sql
    SELECT
    MIN(Date) AS min_date
    , MAX(Date) AS max_date
    FROM [your_project_name_here].sales.sales_info
    ```

    From the query results, you’ll notice that sales_info contains sales from 1/1/2017 to 12/30/2020. Given that you are trying to synthesize an analysis for the sales data, you’ll begin aggregating data in a variety of ways.

    As you work toward understanding this inventory and sales history, you will want to evaluate a few monthly sales stats. One question that you might want to be able to answer is: How many of each product is sold at each store at a given time?

    One way to answer that could be using the following query:

    ```sql
    SELECT
    EXTRACT(YEAR FROM Date) AS YEAR --time grouping
    , EXTRACT(MONTH FROM Date) AS MONTH --time grouping
    , ProductId --need to know which products are sold
    , StoreID --need to know which stores are selling
    , SUM(quantity) AS UnitsSold --how many (impacts inventory)
    , AVG(UnitPrice) AS UnitPriceProxy --can be interesting
    , COUNT(DISTINCT salesID) AS NumTransactions --unique transactions can be interesting
    FROM [your_project_name_here].sales.sales_info
    GROUP BY   YEAR,   MONTH,   ProductId, St
    ```

    This query will return the number of products the retailer sells. But you were also tasked with identifying how this relates to inventory. So, import (upload) the inventory dataset. You can add that as a table right in the sales dataset in BigQuery.

5. Under the actions (three dots) for the sales dataset, select Create Table). You can use these as your settings for the inventory table:

    a. Create table from = UPLOAD (select dropdown option)
    b. Select file = Inventory.csv (select your cleaned inventory file)
    c. Table = inventory (this is the name of the table you’re creating, it won’t have “s)
    d. Schema = Auto detect (select the check box)
    e. Default options on all remaining options.
    f. Select CREATE TABLE.

The previous query can be useful on its own for analysis, but you want to tie that to your newly imported inventory. Use this query:

Note: You’ll need to update your project name in two separate FROM statements.

```sql
with sales_history as (
  SELECT
    EXTRACT(YEAR FROM Date) AS YEAR --time grouping
  , EXTRACT(MONTH FROM Date) AS MONTH --time grouping
  , ProductId --need to know which products are sold
  , StoreID --need to know which stores are selling
  , SUM(quantity) AS UnitsSold --how many (impacts inventory)
  , AVG(UnitPrice) AS UnitPriceProxy --can be interesting
  , COUNT(DISTINCT salesID) AS NumTransactions --unique transactions can be interesting
  FROM [your_project_name_here].sales.sales_info
```

This is a more advanced query! You don’t need to understand how the it functions just yet, but you will definitely be able to use this query’s output.

For each ProductID + StoreId, you will find:

The current inventory of every product for each store

The average monthly quantity of a given product that was sold at that store

Now you’re ready to output a .csv file to bring back to management.

### Step 6: Export results to a spreadsheet

The subset of data in the query should be about 1,000 rows, based on the inventory list. This means that it can be easily exported to a spreadsheet. It’s important to ensure that you and your stakeholders both understand what it is they require (.csv or something else).

Save your results:

1. Within the query results, select SAVE RESULTS.
    Screenshot of SAVE RESULTS selected
2. Choose CSV (Google Drive).
3. Once the job has completed, select GO TO DRIVE.
    Screenshot the GO TO DRIVE option available
4. Using the Open with dropdown, select Google Sheets.
    Screenshot of the Open with button selected, with Google Sheets selected
    There should be about 1,000 rows.

5. Right-click on the sheet tab and rename the sheet inventory_with_avg_monthly_sales.

    Now, you’re ready to share this with your stakeholder!

    Note: If you closely examined the results of the last query, you would have noted that the avg_quantity_sold_in_a_month far exceeds the inventory’s QuantityAvailable in every row. This is where having a dialogue with your supervisor or stakeholder is so critical! At first, it may feel alarming because it seems the inventory at all of the stores are inadequate to meet the needs of the average quantities of their products sold. In such a situation, checking your work and having an open dialogue will allow you to approach your exploratory analysis effectively and deliver something useful to your audience.

### Pro tip: Save the activity templates

Be sure to save a copy of the .csv templates you used to complete this activity. You can use it for further practice or to help you work through your thought processes for similar tasks in a future data analyst role.

## Reflection

### Question 1: In the text box below, consider this question: Why couldn't you analyze the neighborhood of the store that the sale was made in from the sales.csv file?

- Because the neighborhood of all products is 'Mondawmin'. So, there is no difference of neighborhood among products

### Questions 2: In the text box below, write 2-3 sentences (40-60 words) in response to each of the following questions

- Why is being able to make use of  multiple analysis tools useful for some projects?
  - Using multiple tools allows for a more comprehensive approach to data analysis. Spreadsheets offer direct data observation and cleaning, while SQL provides powerful querying capabilities. Combining both enhances flexibility and efficiency, especially in complex projects.
- How is working with data in spreadsheets and with SQL different? How are they similar?
  - Differences: Spreadsheets enable direct interaction and manipulation of data, suitable for smaller datasets. SQL, on the other hand, is a query language for databases, ideal for large datasets and complex queries.
  - Similarities: Both tools share functions like filtering, sorting, and aggregating data. They contribute to data analysis but operate on different scales and have distinct use cases.

> Congratulations on completing this hands-on activity! In this activity, you previewed data in BigQuery to find a useful subset to analyze, imported it to spreadsheets, and analyzed your data! A good response would include that using multiple tools allows you to be more flexible.
>
> Being able to use SQL to create a subset of data to work with in spreadsheets like you did today gives you more options for how you approach your analysis. In upcoming activities, you will have more opportunities to analyze data from beginning to end!
