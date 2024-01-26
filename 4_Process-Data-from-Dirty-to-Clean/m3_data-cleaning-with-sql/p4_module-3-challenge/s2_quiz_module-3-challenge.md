# Cours 4 Module 3 challenge

## Question 1:A data professional analyzes medical data for a health insurance company. The dataset they are working with contains millions of rows of data. What tool would be most efficient for the analyst to use?

- `SQL`
- Spreadsheet
- CSV
- Word processor

## Question 2:A data analyst discovers that their database has recognized product price data as text strings. What SQL function can the analyst use to convert the text strings to floats?

- TRIM
- LENGTH
- `CAST`
- SUBSTR

## Question 3:Fill in the blank: A data analyst working on a marketing project uses the SQL command _____ to add a row for a recent product lead to their organization’s database

- UPDATE
- CREATE TABLE IF NOT EXISTS
- `INSERT INTO`
- DROP TABLE IF EXISTS

## Question 4:You are working with a database table that has columns about ice cream, such as ice_cream_flavor. Which SUBSTR function and AS command will retrieve the first 4 characters of each flavor and store the result in a new column called flavor_ID?

- `SUBSTR(ice_cream_flavor, 1, 4) AS flavor_ID`
- SUBSTR(ice_cream_flavor 1, 4, AS) flavor_ID
- SUBSTR(ice_cream_flavor, 4) AS flavor_ID
- SUBSTR(1, 4) ice_cream_flavor, AS flavor_ID

## Question 5:In SQL, what function can be used to remove duplicate spaces from a piece of data?

- SUBSTR
- AVG
- `TRIM`
- FORMAT

## Question 6: While working with a database table that contains the column computer_model, you notice that there are some duplicate entries. Which SQL clause would you use in a query to return the computer_model data without these duplicates?

- DELETE computer_model
- DROP computer_model
- `DISTINCT computer_model`
- DUPLICATE computer_model

## Question 7: Fill in the blank: A data analyst uses the SQL command _____ to remove unnecessary tables so they do not clutter their organization’s database

- `DROP TABLE IF EXISTS`
- UPDATE
- INSERT INTO
- CREATE TABLE IF NOT EXISTS

## Question 8: You are using a database table that includes the column credit_card_numbers, and you want to check for any fraudulent activity. Which SQL clause will help you identify any credit card numbers that are more than 16 characters long?

- COUNT(credit_card_numbers) > 16
- WHERE(credit_card_numbers) < 16
- IDENTIFY(credit_card_numbers) < 16
- `LENGTH(credit_card_numbers) > 16`

## Question 9:After joining multiple tables containing data about patient visits to a hospital, you find a significant number of null values in the patient_intake column. What SQL function can you use to replace these null values with a value in a different column?

- `COALESCE`
- CONCAT
- TRIM
- CAST
