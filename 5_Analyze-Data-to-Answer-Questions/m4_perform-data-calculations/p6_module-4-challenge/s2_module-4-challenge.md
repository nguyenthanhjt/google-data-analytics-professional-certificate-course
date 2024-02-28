# Practice Quiz: Test your knowledge on using SQL with temporary tables

**Question 1**
A data analyst at a recycling company manually recalculates the new column materials_sorter. They want to identify any rows with values that do not match those in the original column, compost_sorter. Which SQL clauses would enable them to do so? Select all that apply.

1. **WHERE materials_sorter <> compost_sorter**
2. WHERE materials_sorter !! compost_sorter
3. WHERE materials_sorter >< compost_sorter
4. **WHERE materials_sorter != compost_sorter**

**Question 2**
Fill in the blank: The SQL command GROUP BY groups table rows with _____ values into summary rows.

1. increasing
2. **the same**
3. decreasing
4. null

**Question 3**
What will this spreadsheet function return?

`=SUMIF(E2:E10, ”>=50”, F2:F10)`

1. The count of the number of cells in the array E2:E10 that have a value greater than or equal to 50.
2. **The sum of all values in cells F2 to F10 that correspond to values in cells E2 to E10 that are greater than or equal to 50.**
3. The sum of all values in cells E2 to E10 for which the value in cells F2 to F10 is greater than or equal to 50.
4. The sum of any values in cells E2 to E10 and cells F2 to F10 that are greater than or equal to 50.

**Question 4**
Which of the following statements accurately describe pivot tables? Select all that apply.

1. The rows of a pivot table organize and display values vertically.
2. **The columns of a pivot table organize and display values vertically.**
3. **A pivot table can be used to sort, reorganize, or group data.**
4. **The filters section of a pivot table is used to apply filters based on specific criteria.**

**Question 5**
A data analyst at an engineering company calculates the number of spreadsheet rows that contain the value turbine. Which function do they use?

1. `=COUNTIF(C1:C100,“=turbine”)`
2. `=COUNTIF(C1:C100,turbine)`
3. `=COUNTIF(turbine=C1:C100)`
4. **`=COUNTIF(C1:C100,“turbine”)`**

**Question 6**
Fill in the blank: To copy data from one table into a _____, a data professional uses the SELECT INTO statement.

1. defined function
2. **temporary table**
3. new table
4. table view

**Question 7**
Which SQL statement will create a temporary table?

1. 1

   ```sql
   WITH temp_table FROM (
       SELECT * 
       = orig_table
   );
   ```

2. 2

   ```sql
   SELECT * 
   FROM temp_table;
   ```

3. 3

   ```sql
   CREATE TABLE temp_table AS (
       SELECT orig_table
   );
   ```

4. **Correct**

   ```sql
   WITH temp_table AS (
       SELECT * 
       FROM orig_table WHERE y = 1
   );
   ```

**Question 8**
Which column of the original data was set as a "Value" when making this pivot table?

| time   | COUNT of num_diners |
|--------|----------------------|
| Lunch  | 176                  |
| Dinner | 68                   |
| Grand Total | 244             |

1. (Lunch, Dinner)
2. time
3. `num_diners`: the value is a original column summarized by a calculation function such as: SUM, COUNT, AVG,...
4. COUNT
