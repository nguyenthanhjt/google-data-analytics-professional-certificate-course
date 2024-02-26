# Video - Common calculation formulas

Video transcript

- Welcome back! One of the first calculations most kids learn how to do is counting. Soon after, they learn adding, and that doesn't go away. No matter what age we are, we're always counting or adding something, whether it's change at the grocery store or measurements in a recipe. Data analysts do a lot of counting and adding too. And with the amount of data you'll come across as a data analyst, you'll be grateful to have functions that can do the counting and adding for you. So let's learn how these functions COUNTIF and SUMIF can help you do calculations for your analysis more easily and accurately. We'll start with the COUNTIF function. You might remember COUNTIF from some of the earlier videos about data cleaning. COUNTIF returns the number of cells that match a specified value. Earlier, we showed how COUNTIF can be used to find and count errors in a data set.
- Here we'll only be counting. Just a reminder though, while we won't be actively searching for errors in this video, you'll still want to watch out for any data that doesn't look right when doing your own analysis. As a data analyst, you'll look for and fix errors every step of the way.
- For this example, we'll look at a sample of data from an online kitchen supplies retailer.
- Our stakeholders have asked us to answer a few questions about the data to understand more about customer transactions, including the revenue they're bringing in. We've added the questions we need to answer to the spreadsheet.
- We'll set up a simple summary table, which is a table used to summarize statistical information about data. We'll use the questions to create the attributes for our table columns: count, revenue total, and average revenue per transaction.
- Each of our questions ask about transactions with one item or transactions with more than one item, so those will be the observations for our rows.
- We'll make Quantity the heading for our observations.
- We'll also add borders to make the summary table nice and clear.
- The first question asks, How many transactions include exactly one item? To answer this, we'll add a formula using the COUNTIF function in cell G11.
- We'll begin with an equal sign, COUNTIF, and an open parenthesis.
- Column B has data about quantity. So we'll select cells B3 through B50, followed by a comma.
- Next, we need to tell the formula the value that we're looking for in the cells we've selected. We want to tell the data to count the number of transactions if they equal 1. In this case, between quotation marks, we'll type an equal sign and the number 1 because that's the exact value we need to count. When we add a closed parenthesis and press enter, we get the total count for transactions with only one item, which is 25. We can follow the same steps to count values greater than one.
- But this time, because we only want values greater than 1, we'll type a greater than sign in our formula inside of an equals sign.
- Getting this information helps us compare the data about quantity.
- Okay, now we need to find out how much total revenue each transaction type brought in. Since the data isn't organized by quantity, we'll use the SUMIF function to help us add the revenue for transactions with one item and with one more item separately. SUMIF is a function that adds numeric data based on one condition. Building a formula with SUMIF is a bit different than one with COUNTIF. They both start the same way with an equal sign and the function, but a SUMIF formula contains the range of cells to be evaluated by your criteria, and the criteria. In other words, SUMIF has a list of cells to check based on the criteria you set in the formula. Then the range where we want to add the numbers is placed in the formula if that range is different from the range being evaluated. There's commas between each of these parts. Adding a space after each comma is optional. So let's try this. In cell H11, we'll type our formula.
- The range to be evaluated is in column B, so we'll select those cells.
- The condition we want the data to meet is for the values in the column to be equal to one. So we'll type a comma and then inside quotes an equal sign and the number one.
- Then we'll select the range to be added based on whether the data from our first range is equal to one. This range is in column C, which lists the revenue for each transaction.
- So every amount of revenue earned from a transaction with only one item will be added together. And there's our total. Since this is revenue, we'll change the format of the number to currency, so it shows up as dollars and cents.
- So the transactions with exactly one item earned $1,555.00 in revenue. Let's see how much the transactions with more than one item earned.
- Okay, let's check out the results. Just like with our COUNTIF examples, the second SUMIF formula will be the same as the first, except for the condition, which will make it greater than one.
- When we run the formula, we discover that the revenue total is much higher, $4,735.00. This makes sense, since the revenue is coming from transactions with more than one item. Good news. To complete our objective, we'll do two more quick calculations. First, we'll find the average revenue per transaction by dividing each total by its count. This will show our stakeholders how much of a difference there is in revenue per transaction between one item and multiple item transactions. This information could be useful for lots of reasons. For example, figuring out whether to add a discount on purchases with more than one item to encourage customers to buy more. We'll put these calculations in the last column of our summary table. You might remember that we use a slash in a formula as the operator for division calculations.
- The average revenue for transactions with one item is $62.20.
- And the average revenue for transactions with more than one item is $205.87. And that's it for our analysis. Our summary table now gives the stakeholders and team members a snapshot of the analysis that's easy to understand. Our COUNTIF and SUMIF functions played a big role here. Using these functions to complete calculations, especially in large datasets, can help speed up your analysis. They can also make counting and adding a little more interesting. Nothing wrong with that. And coming up, we'll explore more functions to make your calculations run smoothly. Bye for now.

## Questions and notes

- **Summary table**: A table used to summarize statistical information about data
- **SUMIF**: a function that adds numeric data based on one condition
  - `SUMIF(range, criteria/condition,[sum_range])`

### Question 1: A data analyst is using the following formula: =COUNTIF(C2:C50, “=100”). Which part of the formula defines the value condition that the data must meet in order to be counted?

- `=100` - Correct
- COUNTIF
- C2
- C50

> In the formula =COUNTIF(C2:C50, “=100”), “=100” defines the value condition that the data must meet in order to be counted. In this formula, cells C2 through C50 will be counted if their value equals 100.

## Key points from the video

1. **Introduction to COUNTIF and SUMIF Functions:**
   - Data analysts frequently perform counting and adding operations.
   - Introduction to the COUNTIF and SUMIF functions, which aid in making calculations more efficient and accurate.

2. **Use of COUNTIF Function:**
   - Recap of the COUNTIF function, previously discussed in data cleaning videos.
   - COUNTIF returns the number of cells that match a specified value.
   - Demonstration using a sample dataset from an online kitchen supplies retailer.

3. **Setting Up a Summary Table:**
   - Introduction of a summary table to answer specific questions about customer transactions.
   - Attributes for table columns: count, revenue total, and average revenue per transaction.
   - Quantity is chosen as the heading for observations.

4. **COUNTIF for Transaction Quantity:**
   - Calculation of the number of transactions with exactly one item using the COUNTIF function.
   - Application of the same approach for transactions with more than one item.

5. **SUMIF Function for Revenue Calculation:**
   - Introduction of the SUMIF function, which adds numeric data based on a specified condition.
   - Distinction from COUNTIF: SUMIF includes a range of cells to be evaluated and a range to be added.
   - Demonstration of using SUMIF to calculate revenue for transactions with one item and more than one item.

6. **Formatting and Results:**
   - Formatting revenue as currency for better presentation.
   - Comparison of revenue totals for transactions with one item and more than one item.

7. **Average Revenue Calculation:**
   - Introduction of average revenue per transaction as an additional metric.
   - Calculation using the formula (total revenue / count) for both transaction types.

8. **Conclusion:**
   - Summary table provides stakeholders with a clear snapshot of the analysis.
   - COUNTIF and SUMIF functions play a crucial role in making calculations efficient, especially in large datasets.
