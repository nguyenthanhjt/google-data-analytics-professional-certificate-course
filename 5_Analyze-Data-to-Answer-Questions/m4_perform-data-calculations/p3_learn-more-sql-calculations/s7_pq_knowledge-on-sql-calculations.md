# Practice Quiz: Test your knowledge on SQL calculations

1. **Question 1:** In a SQL query, what is the purpose of the modulo (%) operator?

   - `Return the remainder of a division calculation`
   - Convert a decimal to a percent
   - Apply an exponent to a value
   - Find the square root of a number

    > Correct: The modulo operator returns the remainder of a division calculation.

2. **Question 2:** A data professional writes a query that uses more than one arithmetic operator. What do they add to the query to control the order of the calculations?

   - Colon [:]
   - `Parenthesis [()]`
   - Dollar sign ($)
   - Backslash [/]

    > Correct: They add parentheses to control the order of the calculations.
3. **Question 3:** Spreadsheet cell D5 contains the decimal .74. Which formula will convert it to a percentage?

   - =D5%100
   - =D5(100)
   - =D5*100
   - =D5,100

    > Correct: The formula `=D5*100` will convert it to a percentage, 74%.

4. **Question 4:** What will GROUP BY do in this query?

   ```sql
   SELECT apartment, AVG(price) AS apt_prices
   FROM rent_data
   GROUP BY apartment;
   ```

   - Group only the rows in the apt_prices table
   - Group together the rent_data by apartment prices
   - Group the rows in the table by apartment
   - Group together the apartment and rent_data tables

    > Correct: `GROUP BY` will group the rows in the table by apartment. This query calculates the average price for each apartment, putting the results in a new column called apt_prices.
