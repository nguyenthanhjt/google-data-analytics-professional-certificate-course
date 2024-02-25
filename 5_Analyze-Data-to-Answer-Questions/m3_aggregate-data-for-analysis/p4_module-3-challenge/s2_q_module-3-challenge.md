# Module 3 challenge

## Question 1: While using VLOOKUP, you encounter an error because some of your spreadsheet values have leading and trailing spaces. What function should you use to eliminate these spaces?

- `TRIM`
- VALUE
- CUT
- NOSPACE

## Question 2: Fill in the blank: The spreadsheet function _____ can be used to tally the number of cells in a range that are not empty

- RANGE
- RETURN
- `COUNT`
- COUNT DISTINCT

## Question 3: A data professional writes the following formula: =SUM($A$6:$A$60). What are the purposes of the dollar signs ($) ? Select all that apply

- `Sum the values in cells A6 to A60 regardless of whether the formula is copied.`
- `Ensure rows and columns do not change.`
- `Create an absolute reference.`
- Perform the calculation more efficiently.

## Question 4 What will this query return?

```sql
SELECT *
FROM Equipment_table
LEFT JOIN Computer_table
```

- `All records in the equipment table and any matching rows from the computer table`
- All records in the computer table and any matching rows from the equipment table
- All rows from the equipment table joined together with the computer table
- All records in both the equipment table and the computer table

## Question : In this spreadsheet, which function will search for the water type of Lake Urmia?

```plaintext
A             B             C
Lake          Surface area  Water type
Urmia         2,320         Freshwater
```

- =VLOOKUP(Urmia, A2:C10, 2, false)
- `=VLOOKUP("Urmia", A2:C10, 3, false)`
- =VLOOKUP("Urmia", B2:C10, 2, false)
- =VLOOKUP(Urmia, A2:B10, false)

## Question 6: Fill in the blank: A SQL clause containing HAVING adds a _____ to a query instead of the underlying table

- `filter`
- limit
- join
- subquery

## Question 7: A data analyst at a retail store works with a spreadsheet containing sales data. In order to calculate sales tax correctly for customer orders, the analyst ensures all amounts are converted to numeric values. What function do they use?

- EXCHANGE
- PROCESS
- `VALUE`
- CONVERT

## Question 8: Which query will select all columns from the operations table and alias them to ops?

- `Query 1`: correct

    ```sql
    SELECT *
    FROM operations AS ops
    ```

- Query 2:

    ```sql
    SELECT *
    FROM operations NEW ops
    ```

- Query 3:

    ```sql
    SELECT *
    FROM operations TO ops
    ```

- Query 4:

    ```sql
    SELECT *
    FROM operations ALIAS ops
    ```
