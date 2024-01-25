# Widely used SQL queries

Video Transcript

- Hey, welcome back.
- So far we've learned that SQL has some of the same tools as spreadsheets, but on a much larger scale.
- In this video, we'll learn some of the most widely used SQL queries that you can start using for your own data cleaning and eventual analysis.
- Let's get started.
- We've talked about queries as requests you put into the database to ask it to do things for you.
- Queries are a big part of using SQL.
- It's Structured Query Language, after all.
- Queries can help you do a lot of things, but there are some common ones that data analysts use all the time.
- So let's start there.
- First, I'll show you how to use the SELECT query.
- I've called this one out before, but now I'll add some new things for us to try out.
- Right now, the table viewer is blank because we haven't pulled anything from the database yet.
- For this example, the store we're working with is hosting a giveaway for customers in certain cities.
- We have a database containing customer information that we can use to narrow down which customers are eligible for the giveaway.
- Let's do that now.
- We can use SELECT to specify exactly what data we want to interact with in a table.
- If we combine SELECT with FROM, we can pull data from any table in this database as long as they know what the columns and rows are named.
- We might want to pull the data about customer names and cities from one of the tables.
- To do that, we can input SELECT name, comma, city FROM customer underscore data dot customer underscore address.
- To get this information from the customer underscore address table, which lives in the customer underscore data, data set.
- SELECT and FROM help specify what data we want to extract from the database and use.
- We can also insert new data into a database or update existing data.
- For example, maybe we have a new customer that we want to insert into this table.
- We can use the INSERT INTO query to put that information in.
- Let's start with where we're trying to insert this data, the customer underscore address table.
- We also want to specify which columns we're adding this data to by typing their names in the parentheses.
- That way, SQL can tell the database exactly where we were inputting new information.
- Then we'll tell it what values we're putting in.
- Run the query, and just like that, it added it to our table for us.
- Now, let's say we just need to change the address of a customer.
- Well, we can tell the database to update it for us.
- To do that, we need to tell it we're trying to update the customer underscore address table.
- Then we need to let it know what value we're trying to change.
- But we also need to tell it where we're making that change specifically so that it doesn't change every address in the table.
- There.
- Now this one customer's address has been updated.
- If we want to create a new table for this database, we can use the CREATE TABLE IF NOT EXISTS statement.
- Keep in mind, just running a SQL query doesn't actually create a table for the data we extract.
- It just stores it in our local memory.
- To save it, we'll need to download it as a spreadsheet or save the result into a new table.
- As a data analyst, there are a few situations where you might need to do just that.
- It really depends on what kind of data you're pulling and how often.
- If you're only using a total number of customers, you probably don't need a CSV file or a new table in your database.
- If you're using the total number of customers per day to do something like track a weekend promotion in a store, you might download that data as a CSV file so you can visualize it in a spreadsheet.
- But if you're being asked to pull this trend on a regular basis, you can create a table that will automatically refresh with the query you've written.
- That way, you can directly download the results whenever you need them for a report.
- Another good thing to keep in mind, if you're creating lots of tables within a database, you'll want to use the DROP TABLE IF EXISTS statement to clean up after yourself.
- It's good housekeeping.
- You probably won't be deleting existing tables very often.
- After all, that's the company's data, and you don't want to delete important data from their database.
- But you can make sure you're cleaning up the tables you've personally made so that there aren't old or unused tables with redundant information cluttering the database.
- There.
- Now you've seen some of the most widely used SQL queries in action.
- There's definitely more query keywords for you to learn and unique combinations that'll help you work within databases.
- But this is a great place to start.
- Coming up, we'll learn even more about queries in SQL and how to use them to clean our data.
- See you next time.

## Keypoints

- `SELECT` Query: The SELECT query is essential in SQL, allowing data analysts to specify what data they want to interact with in a table. It combines with FROM to pull data from any table in the database.
- `INSERT INTO` Query: This query is used to insert new data into a database. The instructor demonstrates how to use the INSERT INTO query to add information about a new customer to the customer_address table.
- `UPDATE` Query: The UPDATE query is introduced for modifying existing data. The instructor shows how to update a customer's address in the customer_address table.
- `CREATE TABLE IF NOT EXISTS` Statement: To create a new table within a database, analysts can use the CREATE TABLE IF NOT EXISTS statement. However, running a SQL query doesn't create a table; it stores data in local memory. Saving the table requires downloading it as a spreadsheet or saving the result as a new table.
- **Downloading and Creating Tables**: Depending on the data and its frequency of use, analysts may download results as CSV files for visualization or create tables that automatically refresh with the written query.
- `DROP TABLE IF EXISTS` Statement: It's good practice to use the DROP TABLE IF EXISTS statement to clean up tables created during analysis, ensuring there are no old or unused tables cluttering the database.