# Video: Embed simple calculations with SQL

Video transcript

- Hi again.
- Earlier we showed you how to complete calculations in SQL.
- While there are a few different ways, embedding them in queries is a very useful one.
- When you include a calculation in a query with other commands, you can do more work faster.
- Here's a basic query syntax that we talked about.
- We start with SELECT and then the names of the columns we want to use in our calculations.
- Then we add in calculation details including an operator like a forward slash for division.
- Next, we type AS followed by the new column name to label the column with the calculated values.
- Finally, we end our query with the FROM command and the name of the table that we're pulling data from.
- Now, let's take it to the next level with some embedded calculations that use a syntax like this one.
- Even better, we'll do this with some data about avocados.
- Sorry to those of you who aren't avocado lovers like me.
- Let's get started.
- Feel free to continue watching as we show you the steps using BigQuery.
- If you're joining us, open up your tool of choice for using SQL.
- Be sure to look through the instructions in the reading right before this video to help you get started.
- Data is already loaded, so we can jump right in.
- Our goal is to find out the total number of bags of avocados sold on each date at each location using this data.
- There's already a column that shows us the total, but we want to make sure we understand how that total is calculated.
- We want to make sure that the total column is just small, large, and extra-large bags added together.
- We'll add the values in those three columns together in our query and then compare them to the total bags column in the dataset.
- We'll start with the SELECT command, which we'll use to pull certain columns from the table.
- We are selecting several columns, so we'll press Enter after SELECT and after the comma after each column name.
- Next, we'll type those column names: Date, Region,
- Small_bags, Large_bags, XLarge_Bags, and Total_Bags.
- Underscores are the lines used to underline words and connect text characters.
- Using spaces can confuse certain servers and applications.
- Using underscores instead helps avoid potential issues while keeping the names readable.
- Now we'll add the calculation to the query using the names of the three columns with plus signs between them: small bags plus large bags plus extra large bags.
- Since we want this calculation in a new column, we'll use the AS command to name the column Total_Bags_Calc.
- We've added the word "Calc" so we can compare the columns to each other after we calculate our results.
- Now, we'll finish our query with FROM and the name of the dataset and subset we're pulling from, avocado_data.avocado_prices.
- Let's run the query.
- In the "Total Bags Calc" column, the data shows the sum of each date for the number of small, large, and extra large bags of avocados that were sold at each location.
- If we quickly compare the two columns showing the total number of bags, we learn that the values are the same.
- This lets us know that the data we want to use is the right data.
- Now that we have verified the total number of bags, we can use those values in another query.
- We need to find what percent of the total number of bags were small bags.
- Finding this out might help stakeholders make decisions on how to package avocados or which size bag to run a sale on.
- Our job is to get that information to the stakeholders.
- So we'll set up a new query.
- We'll select the Date, Region, Total Bags, and Small Bags columns for this query.
- Next, we'll set up a new column starting with our calculation.
- To find the percentage of small bags, we need to first divide the number of small bags by the number of total bags using a slash as the operator.
- We'll put this part of the calculation in parentheses to let the server know that this calculation should be performed first.
- Then we'll multiply this total by 100 using an asterisk as our operator.
- Multiplying by 100 gives us a value that's a percentage instead of a decimal.
- Percentages usually make it easier for people to understand quickly when you share results with them.
- We'll use the AS command to name this new column, "Small Bags Percent."
- Then we'll add FROM and the name of the set we're pulling from,
- and we'll run our query.
- We got an error in our results.
- It says that we can't divide by zero.
- Since we're finding percentages, dividing by zero won't work.
- This means that somewhere in the dataset there is total bags equal to zero.
- We'll have to fix this in our query.
- We can fix this using the WHERE command.
- WHERE lets us add a condition to our calculation.
- After we type WHERE, we'll type Total_Bags followed by a less than sign, and then a greater than sign.
- These symbols tell the server that the values we are calculating should not be equal to the value we specify.
- In this case, that value is zero.
- So we'll add a zero to our query.
- Now, when we run the query, you'll notice our new column shows the percent of small bags in the total bags count.
- We'd get the same result if we use an exclamation mark followed by an equal sign in place of the less than and greater than signs.
- Note that this is one way for doing it.
- But there are functions such as SAFE_DIVIDE that also allow you to avoid this error.
- Those are just a couple of examples to get you started.
- But with SQL, you can complete just about any calculation you want during your analysis.
- Embedding the calculations in your queries will help you keep your analysis organized while getting your results.
- The calculation methods we showed you here are just the beginning.
- So look for more coming up.
- See you soon.

## Questions and Notes

### Question 1: When using SQL, which of the following are reasons for using underscores in column names? Select all that apply.

- It tells the server that the values in the columns are for calculations
- `It keeps the column names readable`
- `It helps avoid potential issues with servers and applications`
- It verifies that the values in the columns are accurate

> Using underscores instead of spaces helps avoid potential issues with servers and applications. It also helps to keep the column names readable.
