# Video - Composite functions

Video transcript

- Hi, again.
- Data analysts love discovering new ways to work on their analysis, especially when those new ways simplify their work.
- I know I'm a big fan of learning new tricks to complete tricky tasks.
- Instead of trying to find a new way to do something every time I do an analysis, I try to learn from other people by asking questions and getting help when I need it.
- The people I work with like to use the phrase, stealing with pride.
- All this means is that you should feel no shame for using a process in your analysis that you learned from someone or somewhere else.
- Fellow team members, message board posts, online searches, I've used all of these resources for ideas.
- With pride! Of course, I always cite my sources when I do.
- That's a super important step to remember.
- The SUMPRODUCT function is also one of those tricks that analysts come across either on their own or from another source.
- You can also think of it as a shortcut for doing more complex calculations.
- We'll show you how SUMPRODUCT works and when you might use it to make your work life simpler.
- SUMPRODUCT is a function that multiplies arrays and returns the sum of those products.
- Here's what the SUMPRODUCT formula looks like; equal sign, the SUMPRODUCT followed by an open parenthesis and arrays being multiplied and then added together.
- Each array is separated by a comma.
- An array is kind of like a range in a spreadsheet.
- But keep in mind, an array is a collection of values in cells, not the cells themselves.
- When added to a formula, the SUMPRODUCT function multiplies each of the values in two or more arrays together.
- For example, each value in the array of cells B3 through B7 can be multiplied by its corresponding value in the array of cells C3 through C7.
- B3 times C3, B4 times C4, and so on.
- It will then return the sum of all of those multiplications.
- Let's check out an example using data from a kitchen supplies company.
- You might remember this example from our COUNTIF and SUMIF video.
- We've been given some data about a product order, including the quantity of each product that was sold in the order and the unit price, which tells how much one of each product cost.
- Our job is to use the data in these two columns to find out the total revenue for this order.
- That's where SUMPRODUCT comes in.
- To find the total revenue, we need to do both addition and multiplication calculations.
- First off, we need to find the revenue that each item brought in separately.
- If we did this without SUMPRODUCT, we'd have to multiply each quantity by its unit price: 50 times $1.25, 25 times $5, and so on.
- Then we'd have to add all of those revenue amounts together to get the total revenue.
- Fortunately, the SUMPRODUCT function does all of that for us.
- Let's add the label Total Revenue in cell G5 and then click G6 to input our formula.
- We'll then start our formula with an equal sign and the function followed by an open parenthesis.
- It's good to remind ourselves that the arrays we add to our formula should always be inside the parentheses.
- Next, we'll select cells B3 through B7 for the first array followed by a comma.
- The comma acts as a separator between the two arrays and the formula.
- Then, we'll select cell C3 through C7 for the second array, followed by a closed parenthesis to complete our formula.
- We don't need to include the brackets in our actual formula.
- We included them in the syntax example to clearly define each array for you.
- Then we press Enter to get our total revenue.
- Since we're dealing with revenue, we'll format the number as currency.
- We've learned the total revenue is $655.
- But that's not the actual profit from the sales of these kitchen supplies because we haven't included the profit margin in our calculations.
- The profit margin is a percentage that indicates how many cents of profit have been generated for each dollar of sale.
- In our dataset, product # 789 has a profit margin of 20 percent, meaning each product sold earns a total profit of $0.20 for every dollar.
- And just like the calculation for revenue, we can save time finding profit margin by using the SUMPRODUCT function.
- There's only one difference between the formula for profit margin and revenue in this spreadsheet.
- But it's an important difference.
- To start, in cell G7 we type the same first part of the formula.
- Then we include the two arrays in the same way as well.
- But instead of ending our formula, we add another comma followed by another array.
- This time, we'll select the cells with a profit margin, D3 through D7.
- We'll finish our formula, and our calculation is complete.
- The SUMPRODUCT function saved us from having to multiply each individual revenue amount by each profit margin percentage, then add each profit margin amount together.
- Using SUMPRODUCT for calculations is a time-saver and helps you avoid making mistakes.
- Definitely a trick worth remembering, and there's more worth remembering about calculations coming up next.

## Quetions and Notes

### Notes

- SUMPRODUCT(array1,[array2],...)
- Profit margin: a percentage that indicates how many cents of profit has been generated for each dollar of sale.

- To follow along using the same spreadsheet as the instructor, click the link below and select "Use Template."

Link to template: [Kitchen Supplies, Profit](https://docs.google.com/spreadsheets/d/1tew5mVmK-wkAxJVzS2nZul6IJvK4tdbDfm3IjJfVWsE/template/preview)

OR If you don't have a Google account, you can download the spreadsheet in the attachment [kp-kitchen-supplies---profit.xlsx](./resources/kp-kitchen-supplies---profit.xlsx)

### Question 1: You want to calculate a company’s annual revenue using financial data. You use the SUMPRODUCT function to multiply each of the values in the arrays B3:B7 and C3:C7, then add them together. What is the correct syntax to complete this calculation?

- =SUMPRODUCT+(B3:B7/C3:C7)
- `=SUMPRODUCT(B3:B7,C3:C7)`: correct
- SUMPRODUCT(B3,B7:C3,C7)
- =(SUMPRODUCT)(B3:B7*C3:C7)

> The correct syntax is =SUMPRODUCT(B3:B7,C3:C7). Using this syntax will multiply each value in the first range by its corresponding value in the second range. Then, the values will be added together.
