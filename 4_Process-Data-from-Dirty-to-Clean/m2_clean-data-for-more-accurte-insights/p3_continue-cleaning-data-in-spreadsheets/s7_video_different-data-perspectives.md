# Different data perspectives

VIDEO transcript

- Hi, let's get into it.
- Motivational speaker Wayne Dyer once said, "If you change the way you look at things, the things you look at change." This is so true in data analytics.
- No two analytics projects are ever exactly the same.
- So it only makes sense that different projects require us to focus on different information differently.
In this video, we'll explore different methods that data analysts use to look at data differently and how that leads to more efficient and effective data cleaning.
Some of these methods include sorting and filtering, pivot tables, a function called VLOOKUP, and plotting to find outliers.
Let's start with sorting and filtering.
- As you learned earlier, sorting and filtering data helps data analysts customize and organize the information the way they need for a particular project.
- But these tools are also very useful for data cleaning.
You might remember that sorting involves arranging data into a meaningful order to make it easier to understand, analyze, and visualize.
For data cleaning, you can use sorting to put things in alphabetical or numerical order, so you can easily find a piece of data.
Sorting can also bring duplicate entries closer together for faster identification.
Filters, on the other hand, are very useful in data cleaning when you want to find a particular piece of information.
You learned earlier that filtering means showing only the data that meets a specific criteria while hiding the rest.
This lets you view only the information you need.
When cleaning data, you might use a filter to only find values above a certain number, or just even or odd values.
- Again, this helps you find what you need quickly and separates out the information you want from the rest.
That way you can be more efficient when cleaning your data.
Another way to change the way you view data is by using pivot tables.
You've learned that a pivot table is a data summarization tool that is used in data processing.
Pivot tables sort, reorganize, group, count, total or average data stored in the database.
- In data cleaning, pivot tables are used to give you a quick, clutter- free view of your data.
- You can choose to look at the specific parts of the data set that you need to get a visual in the form of a pivot table.
Let's create one now using our cosmetic makers spreadsheet again.
To start, select the data we want to use.
- Here, we'll choose the entire spreadsheet.
- Select "Data" and then "Pivot table."
Play video starting at :3:5 and follow transcript3:05
Choose "New sheet" and "Create."
Play video starting at :3:11 and follow transcript3:11
Let's say we're working on a project that requires us to look at only the most profitable products.
- Items that earn the cosmetics maker at least $10,000 in orders.
- So the row we'll include is "Total" for total profits.
We'll sort in descending order to put the most profitable items at the top.
And we'll show totals.
Next, we'll add another row for products
Play video starting at :3:49 and follow transcript3:49
so that we know what those numbers are about.
- We can clearly determine tha the most profitable products have the product codes 15143 E-X-F-O and 32729 M-A-S-C.
We can ignore the rest for this particular project because they fall below $10,000 in orders.
Now, we might be able to use context clues to assume we're talking about exfoliants and mascaras.
- But we don't know which ones, or if that assumption is even correct.
So we need to confirm what the product codes correspond to.
And this brings us to the next tool.
- It's called VLOOKUP.
VLOOKUP stands for vertical lookup.
- It's a function that searches for a certain value in a column to return a corresponding piece of information.
- When data analysts look up information for a project, it's rare for all of the data they need to be in the same place.
- Usually, you'll have to search across multiple sheets or even different databases.
The syntax of the VLOOKUP is equals VLOOKUP, open parenthesis, then the data you want to look up.
- Next is a comma and where you want to look for that data.
In our example, this will be the name of a spreadsheet followed by an exclamation point.
The exclamation point indicates that we're referencing a cell in a different sheet from the one we're currently working in.
Again, that's very common in data analytics.
Okay, next is the range in the place where you're looking for data, indicated using the first and last cell separated by a colon.
- After one more comma is the column in the range containing the value to return.
Next, another comma and the word "false," which means that an exact match is what we're looking for.
Finally, complete your function by closing the parentheses.
- To put it simply, VLOOKUP searches for the value in the first argument in the leftmost column of the specified location.
Then the value of the third argument tells VLOOKUP to return the value in the same row from the specified column.
The "false" tells VLOOKUP that we want an exact match.
Soon you'll learn the difference between exact and approximate matches.
- But for now, just know that V lookup takes the value in one cell and searches for a match in another place.
Let's begin.
We'll type equals VLOOKUP.
Then add the data we are looking for, which is the product data.
The dollar sign makes sure that the corresponding part of the reference remains unchanged.
You can lock just the column, just the row, or both at the same time.
Next, we'll tell it to look at Sheet 2, in both columns
Play video starting at :7:33 and follow transcript7:33
We added 2 to represent the second column.
The last term, "false," says we wanted an exact match.
With this information, we can now analyze the data for only the most profitable products.
Going back to the two most profitable products, we can search for 15143 E-X-F-O And 32729 M-A-S-C.
- Go to Edit and then Find.
- Type in the product codes and search for them.
Now we can learn which products we'll be using for this particular project.
The final tool we'll talk about is something called plotting.
- When you plot data, you put it in a graph chart, table, or other visual to help you quickly find what it looks like.
Plotting is very useful when trying to identify any skewed data or outliers.
- For example, if we want to make sure the price of each product is correct, we could create a chart.
- This would give us a visual aid that helps us quickly figure out if anything looks like an error.
So let's select the column with our prices.
Then we'll go to Insert and choose Chart.
Pick a column chart as the type.
- One of these prices looks extremely low.
If we look into it, we discover that this item has a decimal point in the wrong place.
It should be $7.30, not 73 cents.
That would have a big impact on our total profits.
- So it's a good thing we caught that during data cleaning.
Looking at data in new and creative ways helps data analysts identify all kinds of dirty data.
Coming up, you'll continue practicing these new concepts so you can get more comfortable with them.
- You'll also learn additional strategies for ensuring your data is clean, and we'll provide you with effective insights.
- Great work so far.

## Keypoints

- Introduction:
  - Different data analytics projects require different approaches.
  - Wayne Dyer's quote sets the tone: "If you change the way you look at things, the - things you look at change."
- Sorting and Filtering:
  - Sorting and filtering aid in customizing and organizing data for specific projects.
  - Sorting helps arrange data in meaningful order.
  - Filtering shows only data meeting specific criteria, facilitating efficient data - cleaning.
- Pivot Tables:
  - Pivot tables are data summarization tools used in data processing.
  - They provide a clutter-free view of data for quick analysis.
  - Demonstrated using the Cosmetics Inc. spreadsheet to find most profitable products.
- VLOOKUP Function:
  - VLOOKUP (vertical lookup) searches for a value in a column and returns a - corresponding piece of information.
  - Useful when data needed for a project is spread across multiple sheets or databases.
  - Syntax: =VLOOKUP(value, location, column, false) for exact match searches.
- Example - VLOOKUP:
  - Demonstrated using the Cosmetics Inc. spreadsheet to confirm product codes and - details.
- Plotting for Data Visualization:
  - Plotting involves creating graphs, charts, or visuals to quickly identify skewed data - or outliers.
  - Useful for visually inspecting data, e.g., checking product prices for anomalies.
- Example - Plotting:
  - Using a column chart to visualize product prices and identify anomalies.
  - An example of correcting a price with a misplaced decimal point.
- Conclusion:
  - Analyzing data creatively helps identify dirty data.
  - Continued practice will enhance understanding and comfort with these concepts.
  - Future sessions will cover additional strategies for ensuring clean data.
