# Video: Queries and calculations

Video transcript

- By now, you probably know that there's more than one way to do the daily task of a data analyst.
- Calculations are no exception.
- As we've shown in earlier videos, you can complete the same calculations in lots of different ways in spreadsheets.
- You can also complete them using SQL.
- In this video, we'll give you an overview of how SQL calculations compare to spreadsheet calculations.
- Let's look at the arithmetic operators that are used in both spreadsheets and SQL.
- An operator is a symbol that names the type of operation or calculation to be performed in a formula.
- As you learned earlier, the four basic arithmetic operators in spreadsheet formulas are the plus sign for addition, the minus or hyphen for subtraction, the asterisk for multiplication, and the forward slash for division.
- These same operators calculate data in the same way when writing queries in SQL.
- The operators are embedded in the queries when pulling data from a database.
- Just like spreadsheet formulas, there's a few different ways to perform calculations using queries.
- Let's look at the syntax for one possible query.
- The syntax of a query is its structure.
- It should include all the specific details of the data you want to pull into a new table where those details should be placed.
- If you want to add values from two columns of a table, you start with the SELECT command, followed by the name of your first column, then the name of your second column.
- Then you'd add the names of both columns with a plus sign between them.
- After that, you'd type AS followed by the name you'd like to give the column with the added totals.
- Finally, you then complete your query by typing FROM and then the name of the table that you're pulling the data from.
- Running this query would get you a table showing the two columns whose values are being added together plus a new column showing the sums of those values.
- The operator in this query is a plus sign since values are being added.
- If you needed to subtract, multiply, or divide, you'd follow the same steps using the appropriate operators.
- If you need to use more than one arithmetic operator in a calculation, you'd use parentheses to control the order of the calculations.
- If we included column C in our query, we could place parentheses around column A plus column B.
- We then add an asterisk if we're multiplying followed by column C.
- This query would return in a new column, the sum of the values in column A and B multiplied by the values in column C.
- Now, let's say you only wanted the remainder from a division calculation.
- Well, you need a different operator for this, the modulo operator.
- The modulo operator is represented by the percent symbol.
- This is an operator that returns the remainder when one number is divided by another.
- In a spreadsheet, you could complete the same calculation using the MOD function.
- This brings us to another similarity between calculations in spreadsheets and SQL.
- A lot of times, you can use functions instead of operators to complete calculations.
- For example, the SUM function can complete addition problems in spreadsheets and SQL.
- The AVERAGE function in a spreadsheet is the same as the AVG function in SQL.
- They both return the average value of a set of numbers.
- In SQL, these functions are considered aggregate functions because they perform a calculation on one or more values and return a single value.
- You'll learn more about how they're used with the GROUP BY command in a query soon.
- Those are the basics of SQL calculations.
- Knowing how to write a query for a calculation is a good first step.
- Stay with us, and you'll learn more about calculations in SQL.
- Bye for now.

## Question and Notes

- Operator: A symbol that names the type of operation or calculation to be performed in a formula.
  - `+`: addition
  - `-`: subtraction
  - `*`: multiplication
  - `/`: division

- Module: an operator (`%`) that returns the remainder ưwhenone number í divided by another. (as `MOD` in G-Sheets)

## **Key Points:**

- Calculations in SQL are similar to spreadsheet calculations.
- Arithmetic operators like plus, minus, asterisk (for multiplication), and forward slash (for division) are used in both spreadsheets and SQL.
- The syntax of a query involves specifying the columns, operators, and functions to perform calculations.
- Examples of basic arithmetic operations include addition, subtraction, multiplication, and division.
- Parentheses are used to control the order of calculations when multiple operators are involved.
- The modulo operator (%) in SQL returns the remainder when one number is divided by another.
- Functions, such as SUM and AVG, can be used in SQL for calculations, similar to spreadsheet functions.
- Aggregate functions like SUM and AVG perform calculations on one or more values and return a single value.
- Functions in SQL are often used with the GROUP BY command in queries.
